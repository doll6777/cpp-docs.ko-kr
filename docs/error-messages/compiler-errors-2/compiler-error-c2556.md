---
title: 컴파일러 오류 C2556
ms.date: 11/04/2016
f1_keywords:
- C2556
helpviewer_keywords:
- C2556
ms.assetid: fc4399ad-45b3-49fd-be1f-0b13956a595a
ms.openlocfilehash: 6b6f08ac52eff355f0857968817a681818e3c3dc
ms.sourcegitcommit: 16fa847794b60bf40c67d20f74751a67fccb602e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/03/2019
ms.locfileid: "74756775"
---
# <a name="compiler-error-c2556"></a>컴파일러 오류 C2556

' identifier ': 오버 로드 된 함수는 반환 형식만 다릅니다.

오버 로드 된 함수의 반환 형식은 같지만 동일한 매개 변수 목록입니다. 오버 로드 된 각 함수에는 고유한 형식 매개 변수 목록이 있어야 합니다.

다음 샘플에서는 C2556를 생성 합니다.

```cpp
// C2556.cpp
// compile with: /c
class C {
   int func();
   double func();   // C2556
   int func(int i);   // ok parameter lists differ
};
```
