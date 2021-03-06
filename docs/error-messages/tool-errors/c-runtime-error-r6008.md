---
title: C 런타임 오류 R6008
ms.date: 11/04/2016
f1_keywords:
- R6008
helpviewer_keywords:
- R6008
ms.assetid: f0f304fc-709a-4843-bc7e-bad1ae0d1649
ms.openlocfilehash: 214b6548cc7a3b880223503c2f3e9222d64212ca
ms.sourcegitcommit: 857fa6b530224fa6c18675138043aba9aa0619fb
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/24/2020
ms.locfileid: "80197395"
---
# <a name="c-runtime-error-r6008"></a>C 런타임 오류 R6008

인수를 위한 공간이 부족 합니다.

> [!NOTE]
> 앱을 실행 하는 동안이 오류 메시지가 표시 되는 경우 내부 메모리 문제가 있기 때문에 앱이 종료 되었습니다. 이 오류가 발생 하는 이유는 여러 가지가 있지만 종종 메모리 부족 상태, 환경 변수에서 사용 하는 메모리 부족 또는 프로그램의 버그로 인 한 것일 수 있습니다.
>
> 이 오류를 해결하려면 다음 단계를 시도할 수 있습니다.
>
> - 실행 중인 다른 응용 프로그램을 닫거나 컴퓨터를 다시 시작 하 여 메모리를 확보 하십시오.
> - 응용 프로그램에 대 한 명령줄 인수의 수와 크기를 줄입니다.
> - **제어판** 의 **앱 및 기능** 또는 **프로그램 및 기능** 페이지를 사용 하 여 프로그램을 복구 하거나 다시 설치 합니다.
> - **제어판** 의 소프트웨어 업데이트에 대 한 **Windows 업데이트** 를 확인 합니다.
> - 앱의 업데이트 된 버전을 확인 합니다. 문제가 지속 되 면 앱 공급 업체에 문의 하세요.

**프로그래머를 위한 정보**

프로그램을 로드 하는 데 충분 한 메모리가 있지만 **argv** 배열을 만들기에는 메모리가 부족 합니다. 이는 메모리 부족 상태 이거나 비정상적으로 큰 명령줄 또는 환경 변수 사용으로 인해 발생할 수 있습니다. 다음 솔루션 중 하나를 고려 합니다.

- 프로그램에 사용할 수 있는 메모리 양을 늘립니다.

- 명령줄 인수의 수와 크기를 줄입니다.

- 불필요 한 변수를 제거 하 여 환경 크기를 줄입니다.
