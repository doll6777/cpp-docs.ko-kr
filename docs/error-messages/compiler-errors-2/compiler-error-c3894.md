---
title: 컴파일러 오류 C3894
ms.date: 11/04/2016
f1_keywords:
- C3894
helpviewer_keywords:
- C3894
ms.assetid: 6d5ac903-1dea-431d-8e3a-cebca4342983
ms.openlocfilehash: c08a7eca473a4ae043879b49266efec6b8afe7b1
ms.sourcegitcommit: 16fa847794b60bf40c67d20f74751a67fccb602e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/03/2019
ms.locfileid: "74749440"
---
# <a name="compiler-error-c3894"></a>컴파일러 오류 C3894

' var ': ' class ' 클래스의 클래스 생성자 에서만 initonly 정적 데이터 멤버를 l-value로 사용할 수 있습니다.

정적 [initonly](../../dotnet/initonly-cpp-cli.md) 데이터 멤버는 선언 시점 또는 정적 생성자에서 l-value로만 사용할 수 있습니다.

인스턴스 (비정적) initonly 데이터 멤버는 선언 시점 또는 인스턴스 (비정적) 생성자에서 l-value로만 사용할 수 있습니다.

다음 샘플에서는 C3894를 생성 합니다.

```cpp
// C3894.cpp
// compile with: /clr
ref struct Y1 {
   initonly static int data_var = 0;

public:
   // class constructor
   static Y1() {
      data_var = 99;   // OK
      System::Console::WriteLine("in static constructor");
   }

   // not the class constructor
   Y1(int i) {
      data_var = i;   // C3894
   }

   static void Test() {}

};

int main() {
   Y1::data_var = 88;   // C3894
   int i = Y1::data_var;
   Y1 ^ MyY1 = gcnew Y1(99);
   Y1::Test();
}
```
