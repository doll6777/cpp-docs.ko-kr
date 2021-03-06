---
title: '레코드 집합: 대량 레코드 추가(ODBC)'
ms.date: 11/04/2016
helpviewer_keywords:
- ODBC recordsets, adding records
- recordsets, adding records
- bulk record additions to recordsets
ms.assetid: 4685f656-14b9-4f10-a1c5-147b2b89a0b4
ms.openlocfilehash: f561cb0275933a973e97ef0518148e81e14a0234
ms.sourcegitcommit: 857fa6b530224fa6c18675138043aba9aa0619fb
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/24/2020
ms.locfileid: "80213020"
---
# <a name="recordset-adding-records-in-bulk-odbc"></a>레코드 집합: 대량 레코드 추가(ODBC)

이 항목은 MFC ODBC 클래스에 적용됩니다.

MFC [CRecordset](../../mfc/reference/crecordset-class.md) 클래스에는 새 레코드를 테이블에 대량으로 추가할 때 효율성을 향상 시키는 새로운 최적화 기능이 있습니다.

> [!NOTE]
> 이 토픽은 대량 행 페치가 구현되지 않은 `CRecordset`에서 파생된 개체에 적용됩니다. 대량 행 페치를 사용 하는 경우 레코드 [집합: 대량 레코드 페치 (ODBC)](../../data/odbc/recordset-fetching-records-in-bulk-odbc.md)를 참조 하세요.

[CRecordset:: Open](../../mfc/reference/crecordset-class.md#open) 멤버 함수 `optimizeBulkAdd`의 *dwOptions* 매개 변수에 대 한 새 옵션은 `Requery` 또는 `Close`를 호출 하지 않고 여러 레코드를 연속으로 추가할 때 성능을 향상 시킵니다. 첫 번째 `Update` 호출 이전에 더티 인 필드만 후속 `AddNew`/`Update` 호출에 대해 더티로 표시 됩니다.

데이터베이스 클래스를 사용 하 여 레코드를 추가, 편집 및 삭제 하는 `::SQLSetPos` ODBC API 함수를 활용 하는 경우에는이 최적화가 필요 하지 않습니다.

ODBC 커서 라이브러리가 로드 되거나 ODBC 드라이버가 `::SQLSetPos`를 통해 추가, 편집 및 삭제를 지원 하지 않는 경우이 최적화는 대량 추가 성능을 향상 시켜야 합니다. 이 최적화를 켜려면 레코드 집합에 대 한 `Open` 호출에서 *dwOptions* 매개 변수를 다음과 같이 설정 합니다.

```
appendOnly | optimizeBulkAdd
```

## <a name="see-also"></a>참고 항목

[레코드 집합(ODBC)](../../data/odbc/recordset-odbc.md)<br/>
[레코드 집합: 레코드 추가, 업데이트 및 삭제(ODBC)](../../data/odbc/recordset-adding-updating-and-deleting-records-odbc.md)<br/>
[레코드 집합: 레코드 잠금(ODBC)](../../data/odbc/recordset-locking-records-odbc.md)
