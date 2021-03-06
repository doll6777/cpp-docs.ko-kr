---
title: __RTDynamicCast
ms.date: 11/04/2016
api_name:
- __RTDynamicCast
api_location:
- msvcr90.dll
- msvcr110.dll
- msvcr120.dll
- msvcrt.dll
- msvcr100.dll
- msvcr80.dll
- msvcr110_clr0400.dll
api_type:
- DLLExport
topic_type:
- apiref
f1_keywords:
- __RTDynamicCast
helpviewer_keywords:
- __RTDynamicCast
ms.assetid: 56aa2d7a-aa47-46ef-830d-e37175611239
ms.openlocfilehash: 238310791baebc941ad23b798adc1ea2e7fffcbb
ms.sourcegitcommit: 1f009ab0f2cc4a177f2d1353d5a38f164612bdb1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/27/2020
ms.locfileid: "87218509"
---
# <a name="__rtdynamiccast"></a>__RTDynamicCast

[dynamic_cast](../cpp/dynamic-cast-operator.md) 연산자의 런타임 구현입니다.

## <a name="syntax"></a>구문

```cpp
PVOID __RTDynamicCast (
   PVOID inptr,
   LONG VfDelta,
   PVOID SrcType,
   PVOID TargetType,
   BOOL isReference
   ) throw(...)
```

#### <a name="parameters"></a>매개 변수

*inptr*<br/>
다형 개체에 대한 포인터입니다.

*VfDelta*<br/>
개체 내 가상 함수 포인터의 오프셋입니다.

*중 유형이*<br/>
`inptr` 매개 변수가 가리키는 개체의 정적 형식입니다.

*TargetType*<br/>
캐스트의 의도된 결과입니다.

*isReference*<br/>
**`true`** input이 참조 이면이 고, **`false`** 입력이 포인터인 경우입니다.

## <a name="return-value"></a>Return Value

성공 하는 경우 적절 한 하위 개체에 대 한 포인터 그렇지 않으면 **NULL**입니다.

## <a name="exceptions"></a>예외

`bad_cast()`에 대한 입력이 참조이고 캐스팅이 실패한 경우 `dynamic_cast<>`입니다.

## <a name="remarks"></a>설명

`inptr`을 `TargetType` 형식의 개체로 변환합니다. `TargetType`이 포인터인 경우 `inptr`의 형식은 포인터여야 하며 `TargetType`이 참조인 경우에는 l 값이어야 합니다. `TargetType`은 포인터, 이전에 정의한 클래스 형식에 대한 참조 또는 void에 대한 포인터여야 합니다.

## <a name="requirements"></a>요구 사항

|루틴에서 반환된 값|필수 헤더|
|-------------|---------------------|
|__RTDynamicCast|rtti.h|
