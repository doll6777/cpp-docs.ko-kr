---
title: 컴파일러 오류 C3033
ms.date: 11/04/2016
f1_keywords:
- C3033
helpviewer_keywords:
- C3033
ms.assetid: 8628b6bb-a650-4ed2-af13-57acd2f7ddbb
ms.openlocfilehash: df3e3f8472d1c274049e686de93488d556ff6f1f
ms.sourcegitcommit: 1f009ab0f2cc4a177f2d1353d5a38f164612bdb1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/27/2020
ms.locfileid: "87232016"
---
# <a name="compiler-error-c3033"></a>컴파일러 오류 C3033

'var': 'clause' 절의 변수는 const 한정 형식이 될 수 없습니다.

특정 절에 전달 된 값은 변수가 될 수 없습니다 **`const`** .

다음 샘플에서는 C3033을 생성합니다.

```cpp
// C3033.cpp
// compile with: /openmp /link vcomps.lib
int main() {
   const int val = 1;
   int val2 = 1;

   #pragma omp parallel reduction(+ : val)   // C3033
   ;

   #pragma omp parallel reduction(+ : val2)   // OK
   ;
}
```
