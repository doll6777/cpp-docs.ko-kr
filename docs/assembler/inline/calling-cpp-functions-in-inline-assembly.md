---
title: 인라인 어셈블리에서 C++ 함수 호출
ms.date: 08/30/2018
helpviewer_keywords:
- functions [C++], calling in inline assembly
- function calls, C++ functions
- function calls, in inline assembly
- Visual C++, functions
- inline assembly, calling functions
- __asm keyword [C++], calling functions
ms.assetid: 1f0d1eb3-54cf-45d5-838d-958188616b38
ms.openlocfilehash: 781b60c8973593039c0fdfa2f457170e95048597
ms.sourcegitcommit: 1f009ab0f2cc4a177f2d1353d5a38f164612bdb1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/27/2020
ms.locfileid: "87192537"
---
# <a name="calling-c-functions-in-inline-assembly"></a>인라인 어셈블리에서 C++ 함수 호출

**Microsoft 전용**

**`__asm`** 블록은 오버 로드 되지 않은 전역 c + + 함수만 호출할 수 있습니다. 오버로드된 전역 C++ 함수 또는 C++ 멤버 함수를 호출하면 컴파일러에서 오류가 발생합니다.

**Extern "C"** 링크로 선언 된 함수를 호출할 수도 있습니다. **`__asm`** 모든 표준 헤더 파일은 **Extern "C"** 링크를 포함 하도록 라이브러리 함수를 선언 하기 때문에 c + + 프로그램 내의 블록은 c 라이브러리 함수를 호출할 수 있습니다.

**Microsoft 전용 종료**

## <a name="see-also"></a>참조

[인라인 어셈블러](../../assembler/inline/inline-assembler.md)<br/>
