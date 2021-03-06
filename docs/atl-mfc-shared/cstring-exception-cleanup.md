---
title: CString 예외 정리
ms.date: 11/04/2016
helpviewer_keywords:
- CString objects, exceptions
- exception handling, cleanup code
ms.assetid: 28b9ce70-be63-4a0d-92a8-44bbfbc95e83
ms.openlocfilehash: 48c8f1c0040236a4f7bf27a2d5ad985ae343c03a
ms.sourcegitcommit: 1f009ab0f2cc4a177f2d1353d5a38f164612bdb1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/27/2020
ms.locfileid: "87222058"
---
# <a name="cstring-exception-cleanup"></a>CString 예외 정리

이전 버전의 MFC에서는 사용 후에 [CString](../atl-mfc-shared/reference/cstringt-class.md) 개체를 정리 하는 것이 중요 했습니다. MFC 버전 3.0 이상에서는 명시적 정리가 더 이상 필요 하지 않습니다.

이제 MFC에서 사용 하는 c + + 예외 처리 메커니즘을 사용 하 여 예외 후 정리에 대해 걱정할 필요가 없습니다. 예외가 catch 된 후 c + +에서 스택을 "해제" 하는 방법에 대 한 설명은 [try, catch 및 throw 문](../cpp/try-throw-and-catch-statements-cpp.md)을 참조 하십시오. C + + 키워드 및 대신 mfc **TRY**CATCH 매크로를 사용 하는 경우에도 / **CATCH** mfc는 **`try`** **`catch`** 아래의 c + + 예외 메커니즘을 사용 하므로 명시적으로 정리할 필요가 없습니다.

## <a name="see-also"></a>참고 항목

[문자열 (ATL/MFC)](../atl-mfc-shared/strings-atl-mfc.md)<br/>
[예외 처리](../mfc/exception-handling-in-mfc.md)
