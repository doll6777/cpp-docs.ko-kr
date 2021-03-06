---
title: MFC 매크로 및 전역
ms.date: 11/04/2016
helpviewer_keywords:
- MFC, global functions and variables
- MFC, macros
- global functions, MFC
- macros, MFC
- global functions [MFC]
- global variables, MFC
- Afx naming convention
- macros
ms.assetid: add4e33f-0e62-4d27-be14-896cb8675d22
ms.openlocfilehash: ed45fc7014bda18887be6dc8fbcdff8ba9a9c5f1
ms.sourcegitcommit: c123cc76bb2b6c5cde6f4c425ece420ac733bf70
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/14/2020
ms.locfileid: "81373051"
---
# <a name="mfc-macros-and-globals"></a>MFC 매크로 및 전역

Microsoft 재단 클래스 라이브러리는 (1) MFC 클래스와 (2) 매크로 및 전역의 두 가지 주요 섹션으로 나눌 수 있습니다. 함수 또는 변수가 클래스의 멤버가 아닌 경우 전역 함수 또는 변수입니다.

MFC 라이브러리와 활성 템플릿 라이브러리(ATL)는 문자열 변환 매크로를 공유합니다. 자세한 내용은 ATL 설명서의 [문자열 변환 매크로를](../../atl/reference/string-conversion-macros.md) 참조하십시오.

MFC 매크로 및 전역은 다음 범주에서 기능을 제공합니다.

## <a name="general-mfc"></a>일반 MFC

- [데이터 형식](data-types-mfc.md)

- [MFC 클래스 개체의 형식 캐스팅](type-casting-of-mfc-class-objects.md)

- [런타임 개체 모델 서비스](run-time-object-model-services.md)

- [진단 서비스](diagnostic-services.md)

- [예외 처리](exception-processing.md)

- [CString 서식 지정 및 메시지 상자 표시](cstring-formatting-and-message-box-display.md)

- [메시지 맵](message-map-macros-mfc.md)

- [위임 및 인터페이스 맵](delegate-and-interface-maps.md)

- [모듈 및 DLL](extension-dll-macros.md)

- [응용 프로그램 정보 및 관리](application-information-and-management.md)

- [표준 명령 및 창 아이디](standard-command-and-window-ids.md)

- [컬렉션 클래스 도우미](collection-class-helpers.md)

- [회색 및 디더비트맵 함수](gray-and-dithered-bitmap-functions.md)

- [표준 대화 상자 데이터 교환(DDX) 루틴](standard-dialog-data-exchange-routines.md)

- [표준 대화 상자 데이터 유효성 검사(DDV) 루틴](standard-dialog-data-validation-routines.md)

- [AFX 메시지](afx-messages.md)

- [도구 모음 컨트롤 스타일](toolbar-control-styles.md)

- [CMFCImagePaintArea::IMAGE_EDIT_MODE 열거형](cmfcimagepaintarea-image-edit-mode-enumeration.md)

## <a name="database"></a>데이터베이스

- MFC [ODBC 클래스에 대한 RFX(레코드 필드 교환) 함수](record-field-exchange-functions.md) 및 [대량 레코드 필드 교환(벌크 RFX) 함수](record-field-exchange-functions.md)

- MFC DAO 클래스에 대한 [레코드 필드 교환(DFX) 함수](record-field-exchange-functions.md)

- [CRecordView 및 CDaoRecordView(MFC](dialog-data-exchange-functions-for-crecordview-and-cdaorecordview.md) ODBC 및 DAO 클래스)에 대한 대화 데이터 교환(DDX) 기능

- [OLE 컨트롤에 대한 대화 상자 데이터 교환(DDX) 기능](dialog-data-exchange-functions-for-ole-controls.md)

- [ODBC(개방형 데이터베이스 연결) API 함수를 직접 호출하는 데 도움이 될 매크로 및 전역](database-macros-and-globals.md)

- [DAO 데이터베이스 엔진 초기화 및 종료](dao-database-engine-initialization-and-termination.md)

## <a name="internet"></a>인터넷

- [글로벌 인터넷 구문 분석 인터넷 URL](internet-url-parsing-globals.md)

## <a name="dhtml--dhtml-event-maps"></a>DHTML / DHTML 이벤트 맵

- [DHTML 대화 상자 데이터 교환 (DDX) 도우미 매크로](ddx-dhtml-helper-macros.md)

- [DHTML 이벤트 맵](dhtml-event-maps.md)

## <a name="ole"></a>OLE

- [OLE 초기화](ole-initialization.md)

- [애플리케이션 제어](application-control.md)

- [디스패치 맵](dispatch-maps.md)

또한 MFC는 MFC 4.0으로 개발된 모든 OLE 컨테이너가 포함된 OLE 컨트롤을 완벽하게 지원할 수 있도록 [AfxEnableControlContainer라는](ole-initialization.md#afxenablecontrolcontainer) 기능을 제공합니다.

## <a name="ole-controls"></a>올레 컨트롤

- [변형 매개 변수 유형 상수](variant-parameter-type-constants.md)

- [형식 라이브러리 액세스](type-library-access.md)

- [속성 페이지](property-pages-mfc.md)

- [이벤트 맵](event-maps.md)

- [이벤트 싱크 맵](event-sink-maps.md)

- [연결 맵](connection-maps.md)

- [OLE 컨트롤 등록](registering-ole-controls.md)

- [클래스 팩터리 및 라이선스](class-factories-and-licensing.md)

- [OLE 컨트롤의 지속성](persistence-of-ole-controls.md)

이 섹션의 첫 번째 부분에서는 이전 범주각각에 대해 간략하게 설명하고 기능에 대한 간략한 설명과 함께 범주의 전역 및 매크로를 나열합니다. 다음은 MFC 라이브러리의 전역 함수, 전역 변수 및 매크로에 대한 설명입니다.

> [!NOTE]
> 많은 전역 함수는 접두사 "Afx"로 시작하지만, 일부, 예를 들어, 대화 상자 데이터 교환 (DDX) 함수 및 많은 데이터베이스 함수는이 규칙을 따르지 않습니다. 모든 전역 변수는 접두사로 "afx"로 시작합니다. 매크로는 특정 접두사로 시작하지 않지만 대문자로 작성됩니다.

## <a name="see-also"></a>참고 항목

[클래스 개요](../../mfc/class-library-overview.md)
