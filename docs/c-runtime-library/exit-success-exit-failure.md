---
title: EXIT_SUCCESS, EXIT_FAILURE
ms.date: 06/25/2018
f1_keywords:
- EXIT_FAILURE
- EXIT_SUCCESS
helpviewer_keywords:
- EXIT_SUCCESS constant
- EXIT_FAILURE constant
ms.assetid: ff2c82cb-c0bb-4556-a812-59aa278bfac5
ms.openlocfilehash: 562c97b62840285719344d124d8df9944bec25cb
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50519173"
---
# <a name="exitsuccess-exitfailure"></a>EXIT_SUCCESS, EXIT_FAILURE

## <a name="required-header"></a>필수 헤더

```c
#include <stdlib.h>
```

## <a name="remarks"></a>설명

[exit](reference/exit-exit-exit.md) 및 [_exit](reference/exit-exit-exit.md) 함수에 대한 인수이자 [atexit](reference/atexit.md) 및 [_onexit](reference/onexit-onexit-m.md) 함수의 반환 값입니다.

|상수|정의된 값|
|-|-|
|EXIT_SUCCESS|0|
|EXIT_FAILURE|1|

## <a name="see-also"></a>참고 항목

[전역 상수](../c-runtime-library/global-constants.md)
