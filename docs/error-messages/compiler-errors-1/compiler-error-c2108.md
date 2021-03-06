---
title: 컴파일러 오류 C2108
ms.date: 11/04/2016
f1_keywords:
- C2108
helpviewer_keywords:
- C2108
ms.assetid: c84f0b47-5e2c-47d2-8edb-427a40e17c36
ms.openlocfilehash: cbbfa865682ac7423fccd9de4212d901f408810f
ms.sourcegitcommit: 1f009ab0f2cc4a177f2d1353d5a38f164612bdb1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/27/2020
ms.locfileid: "87214778"
---
# <a name="compiler-error-c2108"></a>컴파일러 오류 C2108

첨자가 정수 계열 형식이 아닙니다.

배열 첨자가 정수가 아닌 식입니다.

## <a name="example"></a>예제

값 형식의 포인터를 잘못 사용 하 여 **`this`** 형식의 기본 인덱서에 액세스 하는 경우 C2108이 발생할 수 있습니다. 자세한 내용은 [이 포인터의 의미 체계](../../dotnet/how-to-define-and-consume-classes-and-structs-cpp-cli.md#BKMK_Semantics_of_the_this_pointer)를 참조 하세요.

다음 샘플에서는 C2108를 생성 합니다.

```cpp
// C2108.cpp
// compile with: /clr
using namespace System;

value struct B {
   property Double default[Double] {
      Double get(Double data) {
         return data*data;
      }
   }
   void Test() {
      Console::WriteLine("{0}", this[3.3]);   // C2108
      Console::WriteLine("{0}", this->default[3.3]);   // OK
   }
};

int main() {
   B ^ myb = gcnew B();
   myb->Test();
}
```
