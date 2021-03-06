---
title: 미리 정의된 매크로
description: Microsoft C++ 컴파일러의 미리 정의된 전처리기 매크로가 나열 및 설명되어 있습니다.
ms.custom: update_every_version
ms.date: 06/08/2020
f1_keywords:
- ':::no-loc(_ATL_VER):::'
- ':::no-loc(__ATOM__):::'
- ':::no-loc(__AVX__):::'
- ':::no-loc(__AVX2__):::'
- ':::no-loc(__AVX512BW__):::'
- ':::no-loc(__AVX512CD__):::'
- ':::no-loc(__AVX512DQ__):::'
- ':::no-loc(__AVX512F__):::'
- ':::no-loc(__AVX512VL__):::'
- ':::no-loc(_CHAR_UNSIGNED):::'
- ':::no-loc(__CLR_VER):::'
- ':::no-loc(_CONTROL_FLOW_GUARD):::'
- ':::no-loc(__COUNTER__):::'
- ':::no-loc(__cplusplus):::'
- ':::no-loc(__cplusplus_cli):::'
- ':::no-loc(__cplusplus_winrt):::'
- ':::no-loc(_CPPRTTI):::'
- ':::no-loc(_CPPUNWIND):::'
- ':::no-loc(__DATE__):::'
- ':::no-loc(_DEBUG):::'
- ':::no-loc(_DLL):::'
- ':::no-loc(__FILE__):::'
- ':::no-loc(__FUNCDNAME__):::'
- ':::no-loc(__FUNCSIG__):::'
- ':::no-loc(__FUNCTION__):::'
- ':::no-loc(_INTEGRAL_MAX_BITS):::'
- ':::no-loc(_ISO_VOLATILE):::'
- ':::no-loc(_KERNEL_MODE):::'
- ':::no-loc(__LINE__):::'
- ':::no-loc(_M_AMD64):::'
- ':::no-loc(_M_ARM):::'
- ':::no-loc(_M_ARM_ARMV7VE):::'
- ':::no-loc(_M_ARM_FP):::'
- ':::no-loc(_M_ARM64):::'
- ':::no-loc(_M_CEE):::'
- ':::no-loc(_M_CEE_PURE):::'
- ':::no-loc(_M_CEE_SAFE):::'
- ':::no-loc(_M_FP_EXCEPT):::'
- ':::no-loc(_M_FP_FAST):::'
- ':::no-loc(_M_FP_PRECISE):::'
- ':::no-loc(_M_FP_STRICT):::'
- ':::no-loc(_M_IX86):::'
- ':::no-loc(_M_IX86_FP):::'
- ':::no-loc(_M_X64):::'
- ':::no-loc(_MANAGED):::'
- ':::no-loc(_MFC_VER):::'
- ':::no-loc(_MSC_BUILD):::'
- ':::no-loc(_MSC_EXTENSIONS):::'
- ':::no-loc(_MSC_FULL_VER):::'
- ':::no-loc(_MSC_VER):::'
- ':::no-loc(_MSVC_LANG):::'
- ':::no-loc(__MSVC_RUNTIME_CHECKS):::'
- ':::no-loc(_MT):::'
- ':::no-loc(_NATIVE_WCHAR_T_DEFINED):::'
- ':::no-loc(_NO_SIZED_DEALLOCATION):::'
- ':::no-loc(_OPENMP):::'
- ':::no-loc(_PREFAST_):::'
- ':::no-loc(_RESUMABLE_FUNCTIONS_SUPPORTED):::'
- ':::no-loc(_RTC_CONVERSION_CHECKS_ENABLED):::'
- ':::no-loc(__STDC__):::'
- ':::no-loc(__STDC_HOSTED__):::'
- ':::no-loc(__STDCPP_THREADS__):::'
- ':::no-loc(__TIME__):::'
- ':::no-loc(__TIMESTAMP__):::'
- ':::no-loc(__VA_ARGS__):::'
- ':::no-loc(_VC_NODEFAULTLIB):::'
- ':::no-loc(_WCHAR_T_DEFINED):::'
- ':::no-loc(_WIN32):::'
- ':::no-loc(_WIN64):::'
- ':::no-loc(_WINRT_DLL):::'
helpviewer_keywords:
- timestamps, preprocessor macro
- cl.exe compiler, version number
- version numbers, C/C++ compiler (cl.exe)
- macros, predefined C++
- preprocessor, macros
- predefined macros
- ':::no-loc(_ATL_VER)::: macro'
- ':::no-loc(__ATOM__)::: macro'
- ':::no-loc(__AVX__)::: macro'
- ':::no-loc(__AVX2__)::: macro'
- ':::no-loc(__AVX512BW__)::: macro'
- ':::no-loc(__AVX512CD__)::: macro'
- ':::no-loc(__AVX512DQ__)::: macro'
- ':::no-loc(__AVX512F__)::: macro'
- ':::no-loc(__AVX512VL__)::: macro'
- ':::no-loc(_CHAR_UNSIGNED)::: macro'
- ':::no-loc(__CLR_VER)::: macro'
- ':::no-loc(_CONTROL_FLOW_GUARD)::: macro'
- ':::no-loc(__COUNTER__)::: macro'
- ':::no-loc(__cplusplus)::: macro'
- ':::no-loc(__cplusplus_cli)::: macro'
- ':::no-loc(__cplusplus_winrt)::: macro'
- ':::no-loc(_CPPRTTI)::: macro'
- ':::no-loc(_CPPUNWIND)::: macro'
- ':::no-loc(__DATE__)::: macro'
- ':::no-loc(_DEBUG)::: macro'
- ':::no-loc(_DLL)::: macro'
- ':::no-loc(__FILE__)::: macro'
- ':::no-loc(__FUNCDNAME__)::: macro'
- ':::no-loc(__FUNCSIG__)::: macro'
- ':::no-loc(__FUNCTION__)::: macro'
- ':::no-loc(_INTEGRAL_MAX_BITS)::: macro'
- ':::no-loc(_ISO_VOLATILE)::: macro'
- ':::no-loc(_KERNEL_MODE)::: macro'
- ':::no-loc(__LINE__)::: macro'
- ':::no-loc(_M_AMD64)::: macro'
- ':::no-loc(_M_ARM)::: macro'
- ':::no-loc(_M_ARM_ARMV7VE)::: macro'
- ':::no-loc(_M_ARM_FP)::: macro'
- ':::no-loc(_M_ARM64)::: macro'
- ':::no-loc(_M_CEE)::: macro'
- ':::no-loc(_M_CEE_PURE)::: macro'
- ':::no-loc(_M_CEE_SAFE)::: macro'
- ':::no-loc(_M_FP_EXCEPT)::: macro'
- ':::no-loc(_M_FP_FAST)::: macro'
- ':::no-loc(_M_FP_PRECISE)::: macro'
- ':::no-loc(_M_FP_STRICT)::: macro'
- ':::no-loc(_M_IX86)::: macro'
- ':::no-loc(_M_IX86_FP)::: macro'
- ':::no-loc(_M_X64)::: macro'
- ':::no-loc(_MANAGED)::: macro'
- ':::no-loc(_MFC_VER)::: macro'
- ':::no-loc(_MSC_BUILD)::: macro'
- ':::no-loc(_MSC_EXTENSIONS)::: macro'
- ':::no-loc(_MSC_FULL_VER)::: macro'
- ':::no-loc(_MSC_VER)::: macro'
- ':::no-loc(_MSVC_LANG)::: macro'
- ':::no-loc(__MSVC_RUNTIME_CHECKS)::: macro'
- ':::no-loc(_MT)::: macro'
- ':::no-loc(_NATIVE_WCHAR_T_DEFINED)::: macro'
- ':::no-loc(_NO_SIZED_DEALLOCATION)::: macro'
- ':::no-loc(_OPENMP)::: macro'
- ':::no-loc(_PREFAST_)::: macro'
- ':::no-loc(_RESUMABLE_FUNCTIONS_SUPPORTED)::: macro'
- ':::no-loc(_RTC_CONVERSION_CHECKS_ENABLED)::: macro'
- ':::no-loc(__STDC__)::: macro'
- ':::no-loc(__STDC_HOSTED__)::: macro'
- ':::no-loc(__STDCPP_THREADS__)::: macro'
- ':::no-loc(__TIME__)::: macro'
- ':::no-loc(__TIMESTAMP__)::: macro'
- ':::no-loc(__VA_ARGS__)::: macro'
- ':::no-loc(_VC_NODEFAULTLIB)::: macro'
- ':::no-loc(_WCHAR_T_DEFINED)::: macro'
- ':::no-loc(_WIN32)::: macro'
- ':::no-loc(_WIN64)::: macro'
- ':::no-loc(_WINRT_DLL)::: macro'
- ':::no-loc(__func__)::: identifier'
ms.assetid: 1cc5f70a-a225-469c-aed0-fe766238e23f
no-loc:
- ':::no-loc(_ATL_VER):::'
- ':::no-loc(__ATOM__):::'
- ':::no-loc(__AVX__):::'
- ':::no-loc(__AVX2__):::'
- ':::no-loc(__AVX512BW__):::'
- ':::no-loc(__AVX512CD__):::'
- ':::no-loc(__AVX512DQ__):::'
- ':::no-loc(__AVX512F__):::'
- ':::no-loc(__AVX512VL__):::'
- ':::no-loc(_CHAR_UNSIGNED):::'
- ':::no-loc(__CLR_VER):::'
- ':::no-loc(_CONTROL_FLOW_GUARD):::'
- ':::no-loc(__COUNTER__):::'
- ':::no-loc(__cplusplus):::'
- ':::no-loc(__cplusplus_cli):::'
- ':::no-loc(__cplusplus_winrt):::'
- ':::no-loc(_CPPRTTI):::'
- ':::no-loc(_CPPUNWIND):::'
- ':::no-loc(__DATE__):::'
- ':::no-loc(_DEBUG):::'
- ':::no-loc(_DLL):::'
- ':::no-loc(__FILE__):::'
- ':::no-loc(__FUNCDNAME__):::'
- ':::no-loc(__FUNCSIG__):::'
- ':::no-loc(__FUNCTION__):::'
- ':::no-loc(_INTEGRAL_MAX_BITS):::'
- ':::no-loc(_ISO_VOLATILE):::'
- ':::no-loc(_KERNEL_MODE):::'
- ':::no-loc(__LINE__):::'
- ':::no-loc(_M_AMD64):::'
- ':::no-loc(_M_ARM):::'
- ':::no-loc(_M_ARM_ARMV7VE):::'
- ':::no-loc(_M_ARM_FP):::'
- ':::no-loc(_M_ARM64):::'
- ':::no-loc(_M_CEE):::'
- ':::no-loc(_M_CEE_PURE):::'
- ':::no-loc(_M_CEE_SAFE):::'
- ':::no-loc(_M_FP_EXCEPT):::'
- ':::no-loc(_M_FP_FAST):::'
- ':::no-loc(_M_FP_PRECISE):::'
- ':::no-loc(_M_FP_STRICT):::'
- ':::no-loc(_M_IX86):::'
- ':::no-loc(_M_IX86_FP):::'
- ':::no-loc(_M_X64):::'
- ':::no-loc(_MANAGED):::'
- ':::no-loc(_MFC_VER):::'
- ':::no-loc(_MSC_BUILD):::'
- ':::no-loc(_MSC_EXTENSIONS):::'
- ':::no-loc(_MSC_FULL_VER):::'
- ':::no-loc(_MSC_VER):::'
- ':::no-loc(_MSVC_LANG):::'
- ':::no-loc(__MSVC_RUNTIME_CHECKS):::'
- ':::no-loc(_MT):::'
- ':::no-loc(_NATIVE_WCHAR_T_DEFINED):::'
- ':::no-loc(_NO_SIZED_DEALLOCATION):::'
- ':::no-loc(_OPENMP):::'
- ':::no-loc(_PREFAST_):::'
- ':::no-loc(_RESUMABLE_FUNCTIONS_SUPPORTED):::'
- ':::no-loc(_RTC_CONVERSION_CHECKS_ENABLED):::'
- ':::no-loc(__STDC__):::'
- ':::no-loc(__STDC_HOSTED__):::'
- ':::no-loc(__STDCPP_THREADS__):::'
- ':::no-loc(__TIME__):::'
- ':::no-loc(__TIMESTAMP__):::'
- ':::no-loc(__VA_ARGS__):::'
- ':::no-loc(_VC_NODEFAULTLIB):::'
- ':::no-loc(_WCHAR_T_DEFINED):::'
- ':::no-loc(_WIN32):::'
- ':::no-loc(_WIN64):::'
- ':::no-loc(_WINRT_DLL):::'
- ':::no-loc(__func__):::'
ms.openlocfilehash: 1c7b2f18aede84d8067c36537f33261554c16c17
ms.sourcegitcommit: 1f009ab0f2cc4a177f2d1353d5a38f164612bdb1
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/27/2020
ms.locfileid: "87222643"
---
# <a name="predefined-macros"></a>미리 정의된 매크로

Microsoft C/C++ 컴파일러(MSVC)는 언어(C 또는 C++), 컴파일 대상 및 선택된 컴파일러 옵션을 기반으로 특정 전처리기 매크로를 미리 정의합니다.

MSVC는 ANSI/ISO C99 표준과 ISO C++14 및 C++17 표준에 필요한 미리 정의된 전처리기 매크로를 지원합니다. 이 구현에서는 여러 추가 Microsoft 전용 전처리기 매크로도 지원합니다. 일부 매크로는 특정 빌드 환경 또는 컴파일러 옵션의 경우에만 정의됩니다. 별도로 명시된 경우가 아니면 매크로는 **`/D`** 컴파일러 옵션 인수로 지정된 것처럼 변환 단위 전체에서 정의됩니다. 매크로가 정의되는 경우 컴파일하기 전에 전처리기에서 지정한 값으로 매크로가 확장됩니다. 미리 정의된 매크로는 인수를 사용하지 않으며 다시 정의할 수 없습니다.

## <a name="standard-predefined-identifier"></a>미리 정의된 표준 식별자

컴파일러는 ISO C99 및 ISO C++11에 지정된 아래의 미리 정의된 식별자를 지원합니다.

- `:::no-loc(__func__):::` 바깥쪽 함수의 정규화되지 않은 있는 그대로의 이름으로, **`char`** 의 로컬 **정적 생성자** 배열로 된 함수입니다.

    ```cpp
    void example(){
        printf("%s\n", :::no-loc(__func__):::);
    } // prints "example"
    ```

## <a name="standard-predefined-macros"></a>미리 정의된 표준 매크로

컴파일러는 ISO C99 및 ISO C++17 표준에 지정된 아래의 미리 정의된 매크로를 지원합니다.

- `:::no-loc(__cplusplus):::` 변환 단위가 C++로 컴파일되는 경우 정수 리터럴 값으로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(__DATE__):::` 현재 소스 파일의 컴파일 날짜입니다. 날짜는 *Mmm dd yyyy* 형식의 상수 길이 문자열 리터럴입니다. 월 이름 *Mmm*은 CRT(C 런타임 라이브러리) [asctime](../c-runtime-library/reference/asctime-wasctime.md) 함수에서 생성된 약식 월 이름과 동일합니다. 값이 10 미만인 경우 날짜 *dd*의 첫 문자는 공백입니다. 이 매크로는 항상 정의됩니다.

- `:::no-loc(__FILE__):::` 현재 소스 파일의 이름입니다. `:::no-loc(__FILE__):::`는 문자열 리터럴로 확장됩니다. 파일의 전체 경로를 표시하려면 [ **`/FC`** (진단 소스 코드 파일의 전체 경로)](../build/reference/fc-full-path-of-source-code-file-in-diagnostics.md)를 사용합니다. 이 매크로는 항상 정의됩니다.

- `:::no-loc(__LINE__):::` 현재 소스 파일의 정수 줄 번호로 정의됩니다. `:::no-loc(__LINE__):::` 매크로의 값은 `#line` 지시문을 사용하여 변경할 수 있습니다. 이 매크로는 항상 정의됩니다.

- `:::no-loc(__STDC__):::` C로 컴파일되고 [ **`/Za`** ](../build/reference/za-ze-disable-language-extensions.md) 컴파일러 옵션이 지정된 경우에만 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(__STDC_HOSTED__):::` 구현이 전체 필수 표준 라이브러리를 지원하는 ‘호스트된 구현’인 경우 1로 정의됩니다. 그 이외의 경우에는 0으로 정의됩니다.

- `:::no-loc(__STDCPP_THREADS__):::` 프로그램에 실행 스레드가 두 개 이상 포함될 수 있으며 C++로 컴파일되는 경우에만 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(__TIME__):::` 전처리된 변환 단위를 변환하는 시간입니다. 시간은 *hh:mm:ss* 형식의 문자열 리터럴로, CRT [asctime](../c-runtime-library/reference/asctime-wasctime.md) 함수에서 반환하는 시간과 동일합니다. 이 매크로는 항상 정의됩니다.

## <a name="microsoft-specific-predefined-macros"></a>Microsoft 전용 미리 정의된 매크로

MSVC는 아래의 미리 정의된 매크로도 추가로 지원합니다.

- `:::no-loc(__ATOM__):::` [ **`/favor:ATOM`** ](../build/reference/favor-optimize-for-architecture-specifics.md) 컴파일러 옵션이 설정되고 컴파일러 대상이 x86 또는 x64인 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(__AVX__):::` [ **`/arch:AVX`** ](../build/reference/arch-x86.md), [ **`/arch:AVX2`** ](../build/reference/arch-x86.md) 또는 [ **`/arch:AVX512`** ](../build/reference/arch-x86.md) 컴파일러 옵션이 설정되고 컴파일러 대상이 x86 또는 x 64인 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(__AVX2__):::` [ **`/arch:AVX2`** ](../build/reference/arch-x86.md) 또는 [ **`/arch:AVX512`** ](../build/reference/arch-x86.md) 컴파일러 옵션이 설정되고 컴파일러 대상이 x86 또는 x64인 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(__AVX512BW__):::` [ **`/arch:AVX512`** ](../build/reference/arch-x86.md) 컴파일러 옵션이 설정되고 컴파일러 대상이 x86 또는 x64인 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(__AVX512CD__):::` [ **`/arch:AVX512`** ](../build/reference/arch-x86.md) 컴파일러 옵션이 설정되고 컴파일러 대상이 x86 또는 x64인 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(__AVX512DQ__):::` [ **`/arch:AVX512`** ](../build/reference/arch-x86.md) 컴파일러 옵션이 설정되고 컴파일러 대상이 x86 또는 x64인 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(__AVX512F__):::` [ **`/arch:AVX512`** ](../build/reference/arch-x86.md) 컴파일러 옵션이 설정되고 컴파일러 대상이 x86 또는 x64인 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(__AVX512VL__):::` [ **`/arch:AVX512`** ](../build/reference/arch-x86.md) 컴파일러 옵션이 설정되고 컴파일러 대상이 x86 또는 x64인 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_CHAR_UNSIGNED):::` 기본 **`char`** 형식이 부호 없는 형식인 경우 1로 정의됩니다. 이 값은 [ **`/J`** (부호 없는 기본 문자 형식)](../build/reference/j-default-char-type-is-unsigned.md) 컴파일러 옵션이 설정된 경우 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(__CLR_VER):::` 앱을 컴파일하는 데 사용되는 CLR(공용 언어 런타임)의 버전을 나타내는 정수 리터럴로 정의됩니다. 값은 `Mmmbbbbb` 형식으로 인코딩됩니다. 여기서 `M`은 런타임의 주 버전이고, `mm`은 런타임의 부 버전이며, `bbbbb`는 빌드 번호입니다. `:::no-loc(__CLR_VER):::`은 [ **`/clr`** ](../build/reference/clr-common-language-runtime-compilation.md) 컴파일러 옵션이 설정된 경우 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

    ```cpp
    // clr_ver.cpp
    // compile with: /clr
    using namespace System;
    int main() {
       Console::WriteLine(:::no-loc(__CLR_VER):::);
    }
    ```

- `:::no-loc(_CONTROL_FLOW_GUARD):::` [ **`/guard:cf`** (제어 흐름 보호 사용)](../build/reference/guard-enable-control-flow-guard.md) 컴파일러 옵션이 설정된 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(__COUNTER__):::` 0에서 시작하는 정수 리터럴로 확장됩니다. 소스 파일에서 또는 소스 파일의 포함된 헤더에서 사용될 때마다 값이 1씩 증가합니다. `:::no-loc(__COUNTER__):::`는 미리 컴파일된 헤더를 사용하는 경우 해당 상태를 기억합니다. 이 매크로는 항상 정의됩니다.

  다음 예제에서는 `:::no-loc(__COUNTER__):::`를 사용하여 형식이 동일한 세 가지 개체에 고유 식별자를 할당합니다. `exampleClass` 생성자는 매개 변수로 정수를 사용합니다. 애플리케이션은 `main`에서 `:::no-loc(__COUNTER__):::`를 고유 식별자 매개 변수로 사용하여 `exampleClass` 형식의 세 개체를 선언합니다.

    ```cpp
    // macro:::no-loc(__COUNTER__):::.cpp
    // Demonstration of :::no-loc(__COUNTER__):::, assigns unique identifiers to
    // different objects of the same type.
    // Compile by using: cl /EHsc /W4 macro:::no-loc(__COUNTER__):::.cpp
    #include <stdio.h>

    class exampleClass {
        int m_nID;
    public:
        // initialize object with a read-only unique ID
        exampleClass(int nID) : m_nID(nID) {}
        int GetID(void) { return m_nID; }
    };

    int main()
    {
        // :::no-loc(__COUNTER__)::: is initially defined as 0
        exampleClass e1(:::no-loc(__COUNTER__):::);

        // On the second reference, :::no-loc(__COUNTER__)::: is now defined as 1
        exampleClass e2(:::no-loc(__COUNTER__):::);

        // :::no-loc(__COUNTER__)::: is now defined as 2
        exampleClass e3(:::no-loc(__COUNTER__):::);

        printf("e1 ID: %i\n", e1.GetID());
        printf("e2 ID: %i\n", e2.GetID());
        printf("e3 ID: %i\n", e3.GetID());

        // Output
        // ------------------------------
        // e1 ID: 0
        // e2 ID: 1
        // e3 ID: 2

        return 0;
    }
    ```

- `:::no-loc(__cplusplus_cli):::` C++로 컴파일되고 [ **`/clr`** ](../build/reference/clr-common-language-runtime-compilation.md) 컴파일러 옵션이 설정된 경우 정수 리터럴 값 200406으로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다. 정의되는 경우 `:::no-loc(__cplusplus_cli):::`는 변환 단위 전체에 적용됩니다.

    ```cpp
    // cplusplus_cli.cpp
    // compile by using /clr
    #include "stdio.h"
    int main() {
       #ifdef :::no-loc(__cplusplus_cli):::
          printf("%d\n", :::no-loc(__cplusplus_cli):::);
       #else
          printf("not defined\n");
       #endif
    }
    ```

- `:::no-loc(__cplusplus_winrt):::` C++로 컴파일되고 [ **`/ZW`** (Windows 런타임 컴파일)](../build/reference/zw-windows-runtime-compilation.md) 컴파일러 옵션이 설정된 경우 정수 리터럴 값 201009로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_CPPRTTI):::` [ **`/GR`** (런타임 형식 정보 사용)](../build/reference/gr-enable-run-time-type-information.md) 컴파일러 옵션이 설정된 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_CPPUNWIND):::` [ **`/GX`** (예외 처리 사용)](../build/reference/gx-enable-exception-handling.md), [ **`/clr`** (공용 언어 런타임 컴파일)](../build/reference/clr-common-language-runtime-compilation.md) 또는 [ **`/EH`** (예외 처리 모델)](../build/reference/eh-exception-handling-model.md) 컴파일러 옵션 중 하나 이상이 설정된 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_DEBUG):::` [ **`/LDd`** ](../build/reference/md-mt-ld-use-run-time-library.md), [ **`/MDd`** ](../build/reference/md-mt-ld-use-run-time-library.md), 또는 [ **`/MTd`** ](../build/reference/md-mt-ld-use-run-time-library.md) 컴파일러 옵션이 설정된 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_DLL):::` [ **`/MD`** ](../build/reference/md-mt-ld-use-run-time-library.md) 또는 [ **`/MDd`** ](../build/reference/md-mt-ld-use-run-time-library.md)(다중 스레드 DLL) 컴파일러 옵션이 설정된 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(__FUNCDNAME__):::` 바깥쪽 함수의 [데코레이팅된 이름](../build/reference/decorated-names.md)이 포함된 문자열 리터럴로 정의됩니다. 이 매크로는 함수 내에서만 정의됩니다. [ **`/EP`** ](../build/reference/ep-preprocess-to-stdout-without-hash-line-directives.md) 또는 [ **`/P`** ](../build/reference/p-preprocess-to-a-file.md) 컴파일러 옵션을 사용하는 경우 `:::no-loc(__FUNCDNAME__):::` 매크로가 확장되지 않습니다.

   다음 예제에서는 `:::no-loc(__FUNCDNAME__):::`, `:::no-loc(__FUNCSIG__):::` 및 `:::no-loc(__FUNCTION__):::` 매크로를 사용하여 함수 정보를 표시합니다.

   [!code-cpp[NVC_Predefined_Macros_Examples#1](../preprocessor/codesnippet/CPP/predefined-macros_1.cpp)]

- `:::no-loc(__FUNCSIG__):::` 바깥쪽 함수의 시그니처가 포함된 문자열 리터럴로 정의됩니다. 이 매크로는 함수 내에서만 정의됩니다. [ **`/EP`** ](../build/reference/ep-preprocess-to-stdout-without-hash-line-directives.md) 또는 [ **`/P`** ](../build/reference/p-preprocess-to-a-file.md) 컴파일러 옵션을 사용하는 경우 `:::no-loc(__FUNCSIG__):::` 매크로가 확장되지 않습니다. 64비트 대상에 대해 컴파일되는 경우 호출 규칙은 기본적으로 **`__cdecl`** 입니다. 사용 예제는 `:::no-loc(__FUNCDNAME__):::` 매크로를 참조하세요.

- `:::no-loc(__FUNCTION__):::` 바깥쪽 함수의 데코레이트되지 않은 이름이 포함된 문자열 리터럴로 정의됩니다. 이 매크로는 함수 내에서만 정의됩니다. [ **`/EP`** ](../build/reference/ep-preprocess-to-stdout-without-hash-line-directives.md) 또는 [ **`/P`** ](../build/reference/p-preprocess-to-a-file.md) 컴파일러 옵션을 사용하는 경우 `:::no-loc(__FUNCTION__):::` 매크로가 확장되지 않습니다. 사용 예제는 `:::no-loc(__FUNCDNAME__):::` 매크로를 참조하세요.

- `:::no-loc(_INTEGRAL_MAX_BITS):::` 벡터가 아닌 정수 형식의 최대 크기(비트 단위)인 정수 리터럴 값 64로 정의됩니다. 이 매크로는 항상 정의됩니다.

   ```cpp
   // integral_max_bits.cpp
   #include <stdio.h>
   int main() {
      printf("%d\n", :::no-loc(_INTEGRAL_MAX_BITS):::);
   }
   ```

- `__INTELLISENSE__` Visual Studio IDE에서 IntelliSense 컴파일러가 전달하는 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다. 이 매크로는 IntelliSense 컴파일러가 이해하지 못하는 코드를 보호하는 데 사용하거나 해당 빌드와 IntelliSense 컴파일러 간에 전환하는 데 사용할 수 있습니다. 자세한 내용은 [Troubleshooting Tips for IntelliSense Slowness](https://devblogs.microsoft.com/cppblog/troubleshooting-tips-for-intellisense-slowness/)(IntelliSense 속도 저하 문제 해결 팁)를 참조하세요.

- `:::no-loc(_ISO_VOLATILE):::` [ **`/volatile:iso`** ](../build/reference/volatile-volatile-keyword-interpretation.md) 컴파일러 옵션이 설정된 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_KERNEL_MODE):::` [ **`/kernel`** (커널 모드 이진 만들기)](../build/reference/kernel-create-kernel-mode-binary.md) 컴파일러 옵션이 설정된 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_M_AMD64):::` x64 프로세서를 대상으로 하는 컴파일의 경우 정수 리터럴 값 100으로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_M_ARM):::` ARM 프로세서를 대상으로 하는 컴파일의 경우 정수 리터럴 값 7로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_M_ARM_ARMV7VE):::` ARM 프로세서를 대상으로 하는 컴파일에 대해 [ **`/arch:ARMv7VE`** ](../build/reference/arch-arm.md) 컴파일러 옵션이 설정된 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_M_ARM_FP):::` ARM 프로세서 대상의 경우 설정된 [ **`/arch`** ](../build/reference/arch-arm.md) 컴파일러 옵션을 나타내는 정수 리터럴 값으로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

  - **`/arch`** ARM 옵션이 지정되지 않아 ARM의 기본 아키텍처(`VFPv3`)가 설정되었음을 나타내는 경우 30~39 범위의 값입니다.

  - **`/arch:VFPv4`** 가 설정된 경우 40~49 범위의 값입니다.

  - 자세한 내용은 [ **`/arch`** (ARM)](../build/reference/arch-arm.md)를 참조하세요.

- `:::no-loc(_M_ARM64):::` 64비트 ARM 프로세서를 대상으로 하는 컴파일의 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_M_CEE):::` [ **`/clr`** (공용 언어 런타임 컴파일)](../build/reference/clr-common-language-runtime-compilation.md) 컴파일러 옵션이 설정된 경우 001로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_M_CEE_PURE):::` Visual Studio 2015부터는 사용되지 않습니다. [ **`/clr:pure`** ](../build/reference/clr-common-language-runtime-compilation.md) 컴파일러 옵션이 설정된 경우 001로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_M_CEE_SAFE):::` Visual Studio 2015부터는 사용되지 않습니다. [ **`/clr:safe`** ](../build/reference/clr-common-language-runtime-compilation.md) 컴파일러 옵션이 설정된 경우 001로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_M_FP_EXCEPT):::` [ **`/fp:except`** ](../build/reference/fp-specify-floating-point-behavior.md) 또는 [ **`/fp:strict`** ](../build/reference/fp-specify-floating-point-behavior.md) 컴파일러 옵션이 설정된 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_M_FP_FAST):::` [ **`/fp:fast`** ](../build/reference/fp-specify-floating-point-behavior.md) 컴파일러 옵션이 설정된 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_M_FP_PRECISE):::` [ **`/fp:precise`** ](../build/reference/fp-specify-floating-point-behavior.md) 컴파일러 옵션이 설정된 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_M_FP_STRICT):::` [ **`/fp:strict`** ](../build/reference/fp-specify-floating-point-behavior.md) 컴파일러 옵션이 설정된 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_M_IX86):::` x86 프로세서를 대상으로 하는 컴파일의 경우 정수 리터럴 값 600으로 정의됩니다. x64 또는 ARM 컴파일 대상의 경우 이 매크로가 정의되지 않습니다.

- `:::no-loc(_M_IX86_FP):::` 설정된 [ **`/arch`** ](../build/reference/arch-arm.md) 컴파일러 옵션 또는 기본값을 나타내는 정수 리터럴 값으로 정의됩니다. 컴파일 대상이 x86 프로세서인 경우 이 매크로는 항상 정의됩니다. 그 이외의 경우에는 정의되지 않습니다. 정의되는 경우 값은 다음과 같습니다.

  - `/arch:IA32` 컴파일러 옵션이 설정된 경우 0입니다.

  - `/arch:SSE` 컴파일러 옵션이 설정된 경우 1입니다.

  - `/arch:SSE2`, `/arch:AVX`, `/arch:AVX2` 또는 `/arch:AVX512` 컴파일러 옵션이 설정된 경우 2입니다. `/arch` 컴파일러 옵션이 지정되지 않은 경우 이 값이 기본값입니다. `/arch:AVX`가 지정된 경우 `:::no-loc(__AVX__):::` 매크로도 정의됩니다. `/arch:AVX2`가 지정된 경우 `:::no-loc(__AVX__):::` 및 `:::no-loc(__AVX2__):::`도 정의됩니다. `/arch:AVX512`가 지정된 경우 `:::no-loc(__AVX__):::`, `:::no-loc(__AVX2__):::`, `:::no-loc(__AVX512BW__):::`, `:::no-loc(__AVX512CD__):::`, `:::no-loc(__AVX512DQ__):::`, `:::no-loc(__AVX512F__):::` 및 `:::no-loc(__AVX512VL__):::`도 정의됩니다.

  - 자세한 내용은 [ **`/arch`** (x86)](../build/reference/arch-x86.md)를 참조하세요.

- `:::no-loc(_M_X64):::` x64 프로세서를 대상으로 하는 컴파일의 경우 정수 리터럴 값 100으로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_MANAGED):::` [ **`/clr`** ](../build/reference/clr-common-language-runtime-compilation.md) 컴파일러 옵션이 설정된 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_MSC_BUILD):::` 컴파일러 버전 번호의 수정 번호 요소가 포함된 정수 리터럴로 정의됩니다. 수정 번호는 마침표로 구분된 버전 번호의 네 번째 요소입니다. 예를 들어 Microsoft C/C++ 컴파일러의 버전 번호가 15.00.20706.01인 경우 `:::no-loc(_MSC_BUILD):::` 매크로를 실행하면 1이 나옵니다. 이 매크로는 항상 정의됩니다.

- `:::no-loc(_MSC_EXTENSIONS):::` 기본적으로 사용되는 [ **`/Ze`** (언어 확장 사용)](../build/reference/za-ze-disable-language-extensions.md) 컴파일러 옵션이 설정된 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_MSC_FULL_VER):::` 컴파일러 버전 번호의 주 번호, 부 번호 및 빌드 번호 요소를 인코딩하는 정수 리터럴로 정의됩니다. 주 번호는 마침표로 구분된 버전 번호의 첫 번째 요소이며, 부 번호는 두 번째 요소이고, 빌드 번호는 세 번째 요소입니다. 예를 들어 Microsoft C/C++ 컴파일러의 버전 번호가 15.00.20706.01인 경우 `:::no-loc(_MSC_FULL_VER):::` 매크로를 실행하면 150020706이 나옵니다. 컴파일러의 버전 번호를 보려면 명령줄에 `cl /?`를 입력합니다. 이 매크로는 항상 정의됩니다.

- `:::no-loc(_MSC_VER):::` 컴파일러 버전 번호의 주 번호 및 부 번호 요소를 인코딩하는 정수 리터럴로 정의됩니다. 주 번호는 마침표로 구분된 버전 번호의 첫 번째 요소이며, 부 번호는 두 번째 요소입니다. 예를 들어 Microsoft C/C++ 컴파일러의 버전 번호가 17.00.51106.1인 경우 `:::no-loc(_MSC_VER):::` 매크로를 실행하면 1700이 나옵니다. 컴파일러의 버전 번호를 보려면 명령줄에 `cl /?`를 입력합니다. 이 매크로는 항상 정의됩니다.

   | Visual Studio 버전 | `:::no-loc(_MSC_VER):::` |
   |--|--|
   | Visual Studio 6.0 | 1200 |
   | Visual Studio .NET 2002(7.0) | 1300 |
   | Visual Studio .NET 2003(7.1) | 1310 |
   | Visual Studio 2005(8.0) | 1400 |
   | Visual Studio 2008(9.0) | 1500 |
   | Visual Studio 2010(10.0) | 1600 |
   | Visual Studio 2012(11.0) | 1700 |
   | Visual Studio 2013(12.0) | 1800 |
   | Visual Studio 2015(14.0) | 1900 |
   | Visual Studio 2017 RTW(15.0) | 1910 |
   | Visual Studio 2017 15.3 버전 | 1911 |
   | Visual Studio 2017 15.5 버전 | 1912 |
   | Visual Studio 2017 버전 15.6 | 1913 |
   | Visual Studio 2017 버전 15.7 | 1914 |
   | Visual Studio 2017 버전 15.8 | 1915 |
   | Visual Studio 2017 버전 15.9 | 1916 |
   | Visual Studio 2019 RTW(16.0) | 1920 |
   | Visual Studio 2019 버전 16.1 | 1921 |
   | Visual Studio 2019 버전 16.2 | 1922 |
   | Visual Studio 2019 버전 16.3 | 1923 |
   | Visual Studio 2019 버전 16.4 | 1924 |
   | Visual Studio 2019 버전 16.5 | 1925 |
   | Visual Studio 2019 버전 16.6 | 1926 |
   | Visual Studio 2019 버전 16.7 | 1927 |

   Visual Studio의 지정된 버전 이상에서 컴파일러 릴리스 또는 업데이트를 테스트하려면 `>=` 연산자를 사용합니다. 조건부 지시문에서 이 연산자를 사용하여 알려진 버전과 `:::no-loc(_MSC_VER):::`을 비교할 수 있습니다. 비교할 상호 배타적인 버전이 여러 개 있는 경우 버전 번호의 내림차순으로 비교 순서를 지정합니다. 예를 들어 아래 코드는 Visual Studio 2017 이상에서 릴리스된 컴파일러를 확인합니다. 다음으로 Visual Studio 2015 이상에서 릴리스된 컴파일러를 확인합니다. 그런 다음 Visual Studio 2015 이전에 릴리스된 모든 컴파일러를 확인합니다.

   ```cpp
   #if :::no-loc(_MSC_VER)::: >= 1910
   // . . .
   #elif :::no-loc(_MSC_VER)::: >= 1900
   // . . .
   #else
   // . . .
   #endif
   ```

   자세한 내용은 Microsoft C++ 팀 블로그의 [Visual C++ Compiler Version](https://devblogs.microsoft.com/cppblog/visual-c-compiler-version/)(Visual C++ 컴파일러 버전)을 참조하세요.

- `:::no-loc(_MSVC_LANG):::` 컴파일러가 대상으로 하는 C++ 언어 표준을 지정하는 정수 리터럴로 정의됩니다. C++로 컴파일되는 코드에서만 설정됩니다. 기본적으로 또는 [ **`/std:c++14`** ](../build/reference/std-specify-language-standard-version.md) 컴파일러 옵션이 지정된 경우 이 매크로는 정수 리터럴 값 201402L입니다. [ **`/std:c++17`** ](../build/reference/std-specify-language-standard-version.md) 컴파일러 옵션이 지정된 경우 매크로가 201703L로 설정됩니다. [ **`/std:c++latest`** ](../build/reference/std-specify-language-standard-version.md) 옵션이 지정된 경우 지정되지 않은 더 높은 값으로 설정됩니다. 그 이외의 경우에는 매크로가 정의되지 않습니다. Visual Studio 2015 업데이트 3부터 `:::no-loc(_MSVC_LANG):::` 매크로 및 [ **`/std`** (언어 표준 버전 지정)](../build/reference/std-specify-language-standard-version.md) 컴파일러 옵션을 사용할 수 있습니다.

- `:::no-loc(__MSVC_RUNTIME_CHECKS):::` [ **`/RTC`** ](../build/reference/rtc-run-time-error-checks.md) 컴파일러 옵션 중 하나가 설정된 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `_MSVC_TRADITIONAL` 전처리기 규칙 모드 [ **`/experimental:preprocessor`** ](../build/reference/experimental-preprocessor.md) 컴파일러 옵션이 설정된 경우 0으로 정의됩니다. 기본적으로 또는 [ **`/experimental:preprocessor-`** ](../build/reference/experimental-preprocessor.md) 컴파일러 옵션이 설정된 경우 기존 전처리기가 사용 중임을 나타내도록 1로 정의됩니다. `_MSVC_TRADITIONAL` 매크로 및 [ **`/experimental:preprocessor`** (전처리기 적합성 모드 사용)](../build/reference/experimental-preprocessor.md) 컴파일러 옵션은 Visual Studio 2017 버전 15.8부터 사용할 수 있습니다.

   ```cpp
   #if defined(_MSVC_TRADITIONAL) && _MSVC_TRADITIONAL
   // Logic using the traditional preprocessor
   #else
   // Logic using cross-platform compatible preprocessor
   #endif
   ```

- `:::no-loc(_MT):::` [ **`/MD`** 또는 **`/MDd`** (다중 스레드 DLL)](../build/reference/md-mt-ld-use-run-time-library.md) 또는 [ **`/MT`** 또는 **`/MTd`** (다중 스레드)](../build/reference/md-mt-ld-use-run-time-library.md)가 지정된 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_NATIVE_WCHAR_T_DEFINED):::` [ **`/Zc:wchar_t`** ](../build/reference/zc-wchar-t-wchar-t-is-native-type.md) 컴파일러 옵션이 설정된 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_OPENMP):::` [ **`/openmp`** (OpenMP 2.0 지원 활성화)](../build/reference/openmp-enable-openmp-2-0-support.md) 컴파일러 옵션이 설정된 경우 정수 리터럴 200203으로 정의됩니다. 이 값은 MSVC에 의해 구현된 OpenMP 사양의 날짜를 나타냅니다. 그 이외의 경우에는 정의되지 않습니다.

   ```cpp
   // :::no-loc(_OPENMP):::_dir.cpp
   // compile with: /openmp
   #include <stdio.h>
   int main() {
      printf("%d\n", :::no-loc(_OPENMP):::);
   }
   ```

- `:::no-loc(_PREFAST_):::` [ **`/analyze`** ](../build/reference/analyze-code-analysis.md) 컴파일러 옵션이 설정된 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(__TIMESTAMP__):::` 현재 소스 파일의 마지막 수정 날짜 및 시간이 포함되어 있으며 CRT [`asctime`](../c-runtime-library/reference/asctime-wasctime.md) 함수에서 반환하는 약식 상수 길이 형식의 문자열 리터럴(예: `Fri 19 Aug 13:32:58 2016`)로 정의됩니다. 이 매크로는 항상 정의됩니다.

- `:::no-loc(_VC_NODEFAULTLIB):::` [ **`/Zl`** (기본 라이브러리 이름 생략)](../build/reference/zl-omit-default-library-name.md) 컴파일러 옵션이 설정된 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_WCHAR_T_DEFINED):::` 기본 [ **`/Zc:wchar_t`** ](../build/reference/zc-wchar-t-wchar-t-is-native-type.md) 컴파일러 옵션이 설정된 경우 1로 정의됩니다. `:::no-loc(_WCHAR_T_DEFINED):::` 매크로가 정의되어 있어도 **`/Zc:wchar_t-`** 컴파일러 옵션이 설정된 경우 값을 포함하지 않으므로 **`wchar_t`** 는 프로젝트에 포함된 시스템 헤더 파일에 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_WIN32):::` 컴파일 대상이 32비트 ARM, 64비트 ARM, x86 또는 x64인 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_WIN64):::` 컴파일 대상이 64비트 ARM 또는 x64인 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

- `:::no-loc(_WINRT_DLL):::` C++로 컴파일되고 [ **`/ZW`** (Windows 런타임 컴파일)](../build/reference/zw-windows-runtime-compilation.md) 컴파일러 옵션과 [ **`/LD`** 또는 **`/LDd`** ](../build/reference/md-mt-ld-use-run-time-library.md) 컴파일러 옵션이 둘 다 설정된 경우 1로 정의됩니다. 그 이외의 경우에는 정의되지 않습니다.

ATL 또는 MFC 라이브러리 버전을 식별하는 전처리기 매크로는 컴파일러에 미리 정의되어 있지 않습니다. ATL 및 MFC 라이브러리 헤더는 내부적으로 이러한 버전 매크로를 정의합니다. 필요한 헤더가 포함되기 전에 만들어진 전처리기 지시문에서는 해당 매크로가 정의되지 않습니다.

- `:::no-loc(_ATL_VER):::` \<atldef.h>에 ATL 버전 번호를 인코딩하는 정수 리터럴로 정의됩니다.

- `:::no-loc(_MFC_VER):::` \<afxver_.h>에 MFC 버전 번호를 인코딩하는 정수 리터럴로 정의됩니다.

## <a name="see-also"></a>참조

[매크로(C/C++)](../preprocessor/macros-c-cpp.md)<br/>
[전처리기 연산자](../preprocessor/preprocessor-operators.md)<br/>
[전처리기 지시문](../preprocessor/preprocessor-directives.md)
