---
title: 컴파일러 경고 (수준 1) C4124
ms.date: 11/04/2016
f1_keywords:
- C4124
helpviewer_keywords:
- C4124
ms.assetid: c08c3a65-9584-47a1-a147-44f00c4b230e
ms.openlocfilehash: 59860bef108a3cd3e8bbbc6ff0790e17dbdaa0d4
ms.sourcegitcommit: 1f009ab0f2cc4a177f2d1353d5a38f164612bdb1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/27/2020
ms.locfileid: "87214492"
---
# <a name="compiler-warning-level-1-c4124"></a>컴파일러 경고 (수준 1) C4124

스택 검사를 사용 하는 __fastcall 비효율적입니다.

**`__fastcall`** 키워드는 스택 검사를 사용 하도록 설정 하는 데 사용 되었습니다.

**`__fastcall`** 규칙은 더 빠른 코드를 생성 하지만 스택 검사를 수행 하면 코드가 느려집니다. 을 사용 하 **`__fastcall`** 는 경우 **check_stack** pragma 또는/Gs.를 사용 하 여 스택 검사를 해제 합니다.

이 경고는 이러한 조건에서 선언 된 첫 번째 함수에 대해서만 실행 됩니다.
