---
title: is_move_constructible 클래스
ms.date: 10/24/2019
f1_keywords:
- type_traits/std::is_move_constructible
helpviewer_keywords:
- is_move_constructible
ms.assetid: becdf076-7419-488d-a335-78adf2478b9b
ms.openlocfilehash: 5495ac39a98f5c194f19d28ba85a1d59f47dfbb4
ms.sourcegitcommit: 1f009ab0f2cc4a177f2d1353d5a38f164612bdb1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/27/2020
ms.locfileid: "87222383"
---
# <a name="is_move_constructible-class"></a>is_move_constructible 클래스

이동 작업을 사용 하 여 형식을 생성할 수 있는지 여부를 테스트 합니다.

## <a name="syntax"></a>구문

```cpp
template <class T>
struct is_move_constructible;
```

### <a name="parameters"></a>매개 변수

*트*\
평가할 형식입니다.

## <a name="remarks"></a>설명

**`true`** 이동 작업을 사용 하 여 *T* 형식을 생성할 수 있는 경우로 평가 되는 형식 조건자입니다. 이 조건자는 `is_constructible<T, T&&>`와 같습니다. 이동 생성자가 없지만 인수를 수락 하는 복사 생성자가 있는 형식 *T* 는를 `const T&` 충족 `std::is_move_constructible` 합니다.

## <a name="requirements"></a>요구 사항

**헤더:**\<type_traits>

**네임스페이스:** std

## <a name="see-also"></a>참고 항목

[<type_traits>](../standard-library/type-traits.md)
