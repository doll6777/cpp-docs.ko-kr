---
title: 컴파일러 오류 C2264
ms.date: 11/04/2016
f1_keywords:
- C2264
helpviewer_keywords:
- C2264
ms.assetid: 158b72cc-cee9-4a08-bd79-b7a5955345a8
ms.openlocfilehash: df3b51c60a0546ed00a8cba7c6db066792cf50a2
ms.sourcegitcommit: 16fa847794b60bf40c67d20f74751a67fccb602e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/03/2019
ms.locfileid: "74758751"
---
# <a name="compiler-error-c2264"></a>컴파일러 오류 C2264

' function ': 함수 정의 또는 선언에 오류가 있습니다. 함수를 호출 하지 않았습니다.

잘못 된 정의 또는 선언으로 인해 함수를 호출할 수 없습니다.

다음 샘플에서는 C2264를 생성 합니다.

```cpp
// C2264.cpp
struct C {
   // Delete the following line to resolve.
   operator int(int = 0){}   // incorrect declaration
};

struct D {
   operator int(){return 0;}   // OK
};

int main() {
   int i;

   C c;
   i = c;   // C2264

   D d;
   i = d;   // OK
}
```
