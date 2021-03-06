---
title: __vmx_off
ms.date: 09/02/2019
f1_keywords:
- __vmx_off
helpviewer_keywords:
- VMXOFF instruction
- __vmx_off intrinsic
ms.assetid: 78a32d46-9291-406c-b982-a550855aff18
ms.openlocfilehash: 226b5111c2f4f6771ac75d165c80c3e8ae2336af
ms.sourcegitcommit: 6e1c1822e7bcf3d2ef23eb8fac6465f88743facf
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/03/2019
ms.locfileid: "70219589"
---
# <a name="__vmx_off"></a>__vmx_off

**Microsoft 전용**

프로세서에서 .VMX (가상 컴퓨터 확장) 작업을 비활성화 합니다.

## <a name="syntax"></a>구문

```C
void __vmx_off();
```

## <a name="remarks"></a>설명

`__vmx_off` 함수는 `VMXOFF` 컴퓨터 명령에 해당합니다. 이 함수는 게스트 운영 체제 및 해당 애플리케이션과 호스트 가상 머신 모니터의 상호 작용을 지원합니다. 자세한 내용을 보려면 [Intel Corporation](https://software.intel.com/articles/intel-sdm) 사이트에서 "IA-32 Intel 아키텍처용 Intel 가상화 기술 사양" 문서 번호 C97063-002 문서를 검색 하십시오.

## <a name="requirements"></a>요구 사항

|내장 함수|아키텍처|
|---------------|------------------|
|`__vmx_off`|x86, x64|

**헤더 파일** \<intrin.h >

**Microsoft 전용 종료**

## <a name="see-also"></a>참고자료

[컴파일러 내장 함수](../intrinsics/compiler-intrinsics.md)
