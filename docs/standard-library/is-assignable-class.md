---
title: is_assignable 클래스
ms.date: 11/04/2016
f1_keywords:
- type_traits/std::is_assignable
helpviewer_keywords:
- is_assignable
ms.assetid: 53444287-c8be-4ad2-9487-a85c066a4f84
ms.openlocfilehash: 2137f6bfb63e93da2c1367a21f608c113e80d196
ms.sourcegitcommit: 1f009ab0f2cc4a177f2d1353d5a38f164612bdb1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/27/2020
ms.locfileid: "87215727"
---
# <a name="is_assignable-class"></a>is_assignable 클래스

`From` 형식의 값을 `To` 형식에 할당할 수 있는지 여부를 테스트합니다.

## <a name="syntax"></a>구문

```cpp
template <class To, class From>
struct is_assignable;
```

### <a name="parameters"></a>매개 변수

*받는 사람*\
할당을 받는 개체의 형식입니다.

*보낸 사람*\
값을 제공하는 개체의 형식입니다.

## <a name="remarks"></a>설명

평가되지 않은 `declval<To>() = declval<From>()` 식은 올바른 형식이어야 합니다. 및 둘 다 `From` `To` 완전 한 형식, **`void`** 또는 범위를 알 수 없는 배열 이어야 합니다.

## <a name="requirements"></a>요구 사항

**헤더:**\<type_traits>

**네임스페이스:** std

## <a name="see-also"></a>참고 항목

[<type_traits>](../standard-library/type-traits.md)
