---
title: 컴파일러 경고(수준 1) C4650
ms.date: 11/04/2016
f1_keywords:
- C4650
helpviewer_keywords:
- C4650
ms.assetid: 3190b3e3-dcd6-4846-939b-f900ab652b2a
ms.openlocfilehash: e57f1d9acba4a8734339f3b8e538120abe542efc
ms.sourcegitcommit: 857fa6b530224fa6c18675138043aba9aa0619fb
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/24/2020
ms.locfileid: "80199570"
---
# <a name="compiler-warning-level-1-c4650"></a>컴파일러 경고(수준 1) C4650

미리 컴파일된 헤더에 디버깅 정보가 없습니다. 헤더의 전역 기호만 사용할 수 있습니다.

미리 컴파일된 헤더 파일이 Microsoft 기호화 된 디버깅 정보로 컴파일되지 않았습니다.

연결 된 경우 결과 실행 파일 또는 동적 연결 라이브러리 파일에는 미리 컴파일된 헤더에 포함 된 로컬 기호에 대 한 디버깅 정보가 포함 되지 않습니다.

이 경고는 미리 컴파일된 헤더 파일을 [/zi](../../build/reference/z7-zi-zi-debug-information-format.md) 명령줄 옵션을 사용 하 여 다시 컴파일하면 방지할 수 있습니다.
