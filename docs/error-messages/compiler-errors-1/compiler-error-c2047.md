---
title: 컴파일러 오류 C2047
ms.date: 11/04/2016
f1_keywords:
- C2047
helpviewer_keywords:
- C2047
ms.assetid: 686a5a81-3857-4753-84a0-5c2e7149cbee
ms.openlocfilehash: f42a1f1dadcff95934236f153be7df7244bff8cb
ms.sourcegitcommit: 1f009ab0f2cc4a177f2d1353d5a38f164612bdb1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/27/2020
ms.locfileid: "87210581"
---
# <a name="compiler-error-c2047"></a>컴파일러 오류 C2047

기본값이 잘못되었습니다.

키워드는 **`default`** 문에만 나타날 수 있습니다 **`switch`** .

다음 샘플에서는 C2047을 생성합니다.

```cpp
// C2047.cpp
int main() {
   int i = 0;
   default:   // C2047
   switch(i) {
      case 0:
      break;
   }
}
```

해결 방법:

```cpp
// C2047b.cpp
int main() {
   int i = 0;
   switch(i) {
      case 0:
      break;
      default:
      break;
   }
}
```
