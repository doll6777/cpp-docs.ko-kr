---
title: C 런타임 오류 R6019
ms.date: 11/04/2016
f1_keywords:
- R6019
helpviewer_keywords:
- R6019
ms.assetid: 8129923e-7db2-40ee-9602-def9365f8d28
ms.openlocfilehash: b647825b7e856be9dc51a5a652be87a4cc6d0e23
ms.sourcegitcommit: 857fa6b530224fa6c18675138043aba9aa0619fb
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/24/2020
ms.locfileid: "80197264"
---
# <a name="c-runtime-error-r6019"></a>C 런타임 오류 R6019

콘솔 장치를 열 수 없습니다.

> [!NOTE]
> 앱을 실행 하는 동안이 오류 메시지가 표시 되 면 콘솔에 액세스 하려고 했지만 충분 한 권한이 없어 응용 프로그램이 종료 되었습니다. 이 오류가 발생 하는 이유는 여러 가지가 있지만 일반적으로 프로그램을 관리자 권한으로 실행 해야 하거나 프로그램에 버그가 있기 때문입니다.
>
> 이 오류를 해결하려면 다음 단계를 시도할 수 있습니다.
>
> - 관리자 권한으로 프로그램을 실행 합니다.
> - **제어판** 의 **앱 및 기능** 또는 **프로그램 및 기능** 페이지를 사용 하 여 프로그램을 복구 하거나 다시 설치 합니다.
> - **제어판** 의 소프트웨어 업데이트에 대 한 **Windows 업데이트** 를 확인 합니다.
> - 앱의 업데이트 된 버전을 확인 합니다. 문제가 지속 되 면 앱 공급 업체에 문의 하세요.

**프로그래머를 위한 정보**

이 오류는 앱에서 콘솔 함수를 호출 했지만 운영 체제에서 콘솔에 대 한 액세스 권한을 부여 하지 않았기 때문에 발생 합니다. 디버깅 모드를 제외 하 고, 콘솔 함수는 일반적으로 Microsoft Store 앱에서 허용 되지 않습니다. 앱을 실행 하는 데 관리자 권한이 필요한 경우 기본적으로 관리자 권한으로 실행 되도록 설치 해야 합니다.
