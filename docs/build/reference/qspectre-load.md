---
title: /Qspectre-load
description: Microsoft C/C++ 컴파일러 (MSVC)/Qspectre-load 옵션에 대해 설명 합니다.
ms.date: 01/28/2020
helpviewer_keywords:
- /Qspectre-load
ms.openlocfilehash: a766cf9b7eef11b7c5819cbdaa7706ab5b80c608
ms.sourcegitcommit: 0f4ee9056d65043fa5a715f0ad1031c0ed30e2b6
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/05/2020
ms.locfileid: "77035555"
---
# <a name="qspectre-load"></a>/Qspectre-load

모든 로드 명령에 대 한 직렬화 명령의 컴파일러 생성을 지정 합니다. 이 옵션은 **/Qspectre** 플래그를 확장 하 여 로드를 기반으로 가능한 모든 잘못 된 **실행 측 채널 공격** 을 완화 합니다.

## <a name="syntax"></a>구문

> **/Qspectre-load**

## <a name="remarks"></a>설명

**/Qspectre-load** 를 설정 하면 컴파일러가 메모리에서 로드를 검색 하 고 그 다음에 serialize 명령을 삽입 합니다. `RET` 및 `CALL`를 비롯 하 여 메모리를 로드 하는 제어 흐름 명령은 로드 및 제어 흐름 전송으로 분할 됩니다. 부하가 보호 되도록 하기 위해 부하가 다음에 `LFENCE` 됩니다. 컴파일러가 `jmp` 명령과 같은 제어 흐름 명령을 분할할 수 없는 경우가 있습니다. 따라서 대체 완화 기법을 사용 합니다. 예를 들어, 컴파일러는 다음과 같이 LFENCE를 삽입 하기 전에 destructively 아닌 대상을 로드 하는 명령을 추가 하 여 `jmp [rax]`를 완화 합니다.

```asm
    xor rbx, [rax]
    xor rbx, [rax]  ; force a load of [rax]
    lfence          ; followed by an LFENCE
    jmp [rax]
```

**/Qspectre-load** 모든 로드에 대 한 추론을 중지 하기 때문에 성능에 미치는 영향이 높습니다. 완화는 모든 위치에서 적절 하지 않습니다. 보호 하지 않아도 되는 성능에 중요 한 코드 블록이 있는 경우 `__declspec(spectre(nomitigation))`를 사용 하 여 이러한 완화를 해제할 수 있습니다. 자세한 내용은 [__declspec 스펙터](../../cpp/spectre.md)를 참조 하세요.

**/Qspectre-load** 옵션은 기본적으로 해제 되어 있으며 모든 최적화 수준을 지원 합니다.

**/Qspectre-load** 옵션은 Visual Studio 2019 버전 16.5 이상에서 사용할 수 있습니다. 이 옵션은 x86 및 x64 프로세서를 대상으로 하는 컴파일러 에서만 사용할 수 있습니다. ARM 프로세서를 대상으로 하는 컴파일러에서는 사용할 수 없습니다.

### <a name="to-set-this-compiler-option-in-the-visual-studio-development-environment"></a>Visual Studio 개발 환경에서 이 컴파일러 옵션을 설정하려면

1. 프로젝트의 **속성 페이지** 대화 상자를 엽니다. 자세한 내용은 [Visual Studio에서 C++ 컴파일러 및 빌드 속성 설정](../working-with-project-properties.md)을 참조합니다.

2. **구성 속성** > **CC++ /**  > **코드 생성** 속성 페이지를 선택 합니다.

3. **스펙터 완화** 속성의 새 값을 선택 합니다. **확인**을 선택하여 변경 내용을 적용합니다.

### <a name="to-set-this-compiler-option-programmatically"></a>프로그래밍 방식으로 이 컴파일러 옵션을 설정하려면

- <xref:Microsoft.VisualStudio.VCProjectEngine.VCCLCompilerTool.AdditionalOptions%2A>을 참조하세요.

## <a name="see-also"></a>참고 항목

[/Q 옵션 (하위 수준 작업)](q-options-low-level-operations.md)\
[MSVC 컴파일러 옵션](compiler-options.md)\
[MSVC 컴파일러 명령줄 구문](compiler-command-line-syntax.md)
