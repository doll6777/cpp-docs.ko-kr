---
title: 컴파일러 경고(수준 4) C4764
ms.date: 11/04/2016
f1_keywords:
- C4764
helpviewer_keywords:
- C4764
ms.assetid: 7bd4296f-966b-484c-bf73-8dbc8e85b4a9
ms.openlocfilehash: 28672d2271e380f6a8240bff98326d5334a0f98f
ms.sourcegitcommit: 573b36b52b0de7be5cae309d45b68ac7ecf9a6d8
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/10/2019
ms.locfileid: "74989187"
---
# <a name="compiler-warning-level-4-c4764"></a>컴파일러 경고(수준 4) C4764

16바이트를 초과하도록 catch 개체를 맞출 수 없습니다.

16보다 큰 맞춤을 지정했지만 일부 플랫폼에서는 함수에서 예외가 발생할 경우 스택이 16보다 크지 않은 맞춤을 강제로 적용합니다.

## <a name="example"></a>예제

다음 샘플에서는 C4764를 생성합니다.

```cpp
// C4764.cpp
// compile with: /W4 /EHsc
// processor: x64 IPF
#include <stdio.h>

class A
{
public:
    int x;
};

typedef __declspec(align(32)) A ALIGNEDA;

int main()
{
    ALIGNEDA a;
    try
    {
        a.x = 15;
        throw a;
    }
    catch (ALIGNEDA b) // can’t align b to > 16 bytes
    {
        printf_s("%d\n", b.x);
    }
}   // C4764
```
