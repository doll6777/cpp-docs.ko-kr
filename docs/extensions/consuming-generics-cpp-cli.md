---
title: 제네릭 사용(C++/CLI)
ms.date: 10/12/2018
ms.topic: reference
helpviewer_keywords:
- generics [C++], consuming from .NET languages
ms.assetid: e6330ef5-e907-432e-b527-7a22f5899639
ms.openlocfilehash: 303fa73f09220b2139d681bf3109fd843299a900
ms.sourcegitcommit: 857fa6b530224fa6c18675138043aba9aa0619fb
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/24/2020
ms.locfileid: "80172414"
---
# <a name="consuming-generics-ccli"></a>제네릭 사용(C++/CLI)

한 .NET(또는 UWP) 언어로 작성된 제네릭을 다른 언어에서 사용할 수도 있습니다. 템플릿과는 달리, 컴파일된 어셈블리의 제네릭은 여전히 제네릭으로 남아있습니다. 따라서 제네릭 형식이 정의된 어셈블리보다 다른 어셈블리 및 다른 언어로 제네릭 형식을 인스턴스화할 수 있습니다.

## <a name="example"></a>예제

### <a name="description"></a>Description

이 예제에서는 C#에 정의된 제네릭 클래스를 보여 줍니다.

### <a name="code"></a>코드

```csharp
// consuming_generics_from_other_NET_languages.cs
// compile with: /target:library
// a C# program
public class CircularList<ItemType> {
   class ListNode    {
      public ItemType m_item;
      public ListNode next;
      public ListNode(ItemType item) {
         m_item = item;
      }
   }

   ListNode first, last;

   public CircularList() {}

   public void Add(ItemType item) {
      ListNode newnode = new ListNode(item);
      if (first == null) {
         first = last = newnode;
         first.next = newnode;
         last.next = first;
      }
      else {
         newnode.next = first;
         first = newnode;
         last.next = first;
      }
   }

   public void Remove(ItemType item) {
      ListNode iter = first;
      if (first.m_item.Equals( item )) {
         first =
         last.next = first.next;
      }
      for ( ; iter != last ; iter = iter.next )
         if (iter.next.m_item.Equals( item )) {
              if (iter.next == last)
                  last = iter;
              iter.next = iter.next.next;
              return;
          }
   }

   public void PrintAll() {
      ListNode iter = first;
      do {
         System.Console.WriteLine( iter.m_item );
         iter = iter.next;
      } while (iter != last);
   }
}
```

## <a name="example"></a>예제

### <a name="description"></a>Description

이 예제에서는 C#에서 작성된 어셈블리를 사용합니다.

### <a name="code"></a>코드

```cpp
// consuming_generics_from_other_NET_languages_2.cpp
// compile with: /clr
#using <consuming_generics_from_other_NET_languages.dll>
using namespace System;
class NativeClass {};
ref class MgdClass {};

int main() {
   CircularList<int>^ circ1 = gcnew CircularList<int>();
   CircularList<MgdClass^>^ circ2 = gcnew CircularList<MgdClass^>();

   for (int i = 0 ; i < 100 ; i += 10)
      circ1->Add(i);
   circ1->Remove(50);
   circ1->PrintAll();
}
```

```Output
90
80
70
60
40
30
20
10
```

## <a name="see-also"></a>참고 항목

[제네릭](generics-cpp-component-extensions.md)
