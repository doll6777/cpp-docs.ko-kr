---
title: operator&lt;=(&lt;sample container&gt;)
ms.date: 11/04/2016
f1_keywords:
- std::<=
- std.operator<=
- operator<=
- std.<=
- std::operator<=
- <=
helpviewer_keywords:
- operator<=
- operator <=
- <= operator, with specific objects
- <= operator
ms.assetid: 338577dd-dc88-4a2b-9e12-0379c54fc8a2
ms.openlocfilehash: fff370d595afaf4b4692b4166f248b56a72efcb8
ms.sourcegitcommit: 590e488e51389066a4da4aa06d32d4c362c23393
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/21/2019
ms.locfileid: "72689173"
---
# <a name="operatorlt-ltsample-containergt"></a>operator&lt;=(&lt;sample container&gt;)

> [!NOTE]
> 이 항목은 Microsoft C++ 설명서에서 C++ 표준 라이브러리에 사용 되는 컨테이너의 작동 하지 않는 예제로 작성 되었습니다. 자세한 내용은 [C++ 표준 라이브러리 컨테이너](../standard-library/stl-containers.md)를 참조하세요.

오버 로드 **연산자 < =** 클래스 템플릿 [컨테이너](../standard-library/sample-container-class.md)의 두 개체를 비교 합니다.

## <a name="syntax"></a>구문

```cpp
template <class Ty>
bool operator<=(
    const Container <Ty>& left,
    const Container <Ty>& right);
```

## <a name="return-value"></a>반환 값

`!(right < left)`을 반환합니다.

## <a name="see-also"></a>참조

[\<sample container>](../standard-library/sample-container.md)
