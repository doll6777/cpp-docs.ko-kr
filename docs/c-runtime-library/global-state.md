---
title: CRT의 전역 상태
ms.date: 04/02/2020
helpviewer_keywords:
- CRT global state
ms.openlocfilehash: a794f201184c10c11611138d30d14b36b00405a7
ms.sourcegitcommit: ec6dd97ef3d10b44e0fedaa8e53f41696f49ac7b
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 08/25/2020
ms.locfileid: "88845187"
---
# <a name="global-state-in-the-crt"></a>CRT의 전역 상태

CRT (유니버설 C 런타임)의 일부 함수는 전역 상태를 사용 합니다. 예를 들어은 `setlocale()` 숫자 구분 기호, 텍스트 코드 페이지 등에 영향을 주는 전체 프로그램에 대 한 로캘을 설정 합니다.

응용 프로그램 및 OS 간에는 응용 프로그램의 전역 상태가 공유 되지 않습니다. 예를 들어, 응용 프로그램에서 `setlocale()` 를 호출 하는 경우 C 런타임 또는 그 반대로를 사용 하는 모든 OS 구성 요소의 로캘에는 영향을 주지 않습니다.

## <a name="os-specific-versions-of-crt-functions"></a>OS 특정 버전의 CRT 함수

작업에서 전역 상태와 상호 작용 하는 함수에는 접두사가 인 "쌍" 함수가 있습니다 `_o_` . 예를 들어:

- `setlocale()` 앱과 관련 된 전역 상태에 영향을 줍니다.
- `_o_setlocale()` 앱이 아닌 모든 OS 구성 요소에서 공유 하는 전역 상태에 영향을 줍니다.

이러한 "쌍" 함수 간의 유일한 차이점은 전역 CRT 상태를 읽거나 쓸 때 OS 특정 버전 (로 시작 하는 버전 `_o_` )은 앱의 전역 상태 복사본 대신 전역 상태의 os 복사본을 사용 한다는 것입니다.

이러한 함수의 OS 특정 버전은에 `ucrt.osmode.lib` 있습니다. 예를 들어 OS 특정 버전 `setlocale()` 은 `_o_setlocale()`

앱의 CRT 상태에서 구성 요소의 CRT 상태를 격리 하는 방법에는 두 가지가 있습니다.

- 컴파일러 옵션/MT (release) 또는 MTd (디버그)를 사용 하 여 구성 요소를 정적으로 연결 합니다. 자세한 내용은 [/md,/mt,/LD](../build/reference/md-mt-ld-use-run-time-library.md)을 참조 하세요. 정적 링크는 이진 크기를 크게 늘릴 수 있습니다.
- Windows 10 20H2부터 CRT에 동적으로 연결 하 여 CRT 상태 격리를 가져오고 OS 모드 내보내기 ( _o_로 시작 되는 함수)를 호출 합니다. OS 모드 내보내기를 호출 하려면 이전 처럼 정적으로 링크 되지만 링커 옵션 (릴리스) 또는 (디버그)를 사용 하 여 정적 다중 항목 RT를 무시 합니다 `/NODEFAULTLIB:libucrt.lib` `/NODEFAULTLIB:libucrtd.lib` . 자세한 내용은 [/Nodefaultlib (라이브러리 무시)](../build/reference/nodefaultlib-ignore-libraries.md) 를 참조 하세요. 및 `ucrt.osmode.lib` 를 링커 입력에 추가 합니다.

> [!Note]
> 소스 코드에서를 쓰지 `setlocale()` 않고 작성 `_o_setlocale()` 합니다. 에 연결 하면 `ucrt.osmode.lib` 링커가 함수의 OS 특정 버전으로 자동으로 대체 됩니다. 즉,는 `setlocale()` 로 대체 됩니다 `_o_setlocale()` .

에 연결 하면 `ucrt.osmode.lib` 앱 모드 에서만 사용할 수 있는 일부 사용이 중지 됩니다. 이러한 호출을 시도 하면 링크 오류가 발생 합니다.

## <a name="global-state-affected-by-appos-separation"></a>앱/OS 분리의 영향을 받는 전역 상태

앱 및 OS 상태 분리의 영향을 받는 전역 상태는 다음과 같습니다.

- [로캘 데이터](locale.md)
- [신호로](reference/signal.md) 설정 된 신호 처리기
- [종료](reference/set-terminate-crt.md) 로 설정 된 종료 루틴
- [errno 및 _doserrno](errno-doserrno-sys-errlist-and-sys-nerr.md)
- [Rand](reference/rand.md) 및 [srand](reference/srand.md) 에서 사용 되는 난수 생성 상태
- 사용자가 해제할 필요가 없는 버퍼를 반환 [_ecvt](reference/ecvt.md) 하는 함수: [strtok, wcstok, _mbstok](reference/strtok-strtok-l-wcstok-wcstok-l-mbstok-mbstok-l.md) [Tmpnam, _wtmpnam](reference/tempnam-wtempnam-tmpnam-wtmpnam.md) [asctime, _wasctime](reference/asctime-wasctime.md) [gmtime, _gmtime32, _gmtime64](reference/gmtime-gmtime32-gmtime64.md) [_fcvt _ecvt](reference/fcvt.md) [strerror, _strerror, _wcserror, __wcserror](reference/strerror-strerror-wcserror-wcserror.md)
- [_Putch에서](reference/putch-putwch.md) 사용 하는 버퍼 _putwch
- [_set_invalid_parameter_handler, _set_thread_local_invalid_parameter_handler](reference/set-invalid-parameter-handler-set-thread-local-invalid-parameter-handler.md)
- [_set_new_handler](reference/set-new-handler.md) 및 [_set_new_mode](reference/set-new-mode.md)
- [fmode] (text-and-binary-mode-file-i-o.md)
- [표준 시간대 정보](time-management.md)

## <a name="see-also"></a>참고 항목

[C 런타임 라이브러리 참조](c-run-time-library-reference.md)
