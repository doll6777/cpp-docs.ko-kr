---
title: tuple_element 클래스
ms.date: 11/04/2016
f1_keywords:
- utility/std::tuple_element
helpviewer_keywords:
- std::tuple_element
ms.assetid: 4c51a6c1-ce81-462f-8c6c-291d69f2b77c
ms.openlocfilehash: 21efed39fdaabe0f95f83e9dc5cdfcc508a147c5
ms.sourcegitcommit: 590e488e51389066a4da4aa06d32d4c362c23393
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/21/2019
ms.locfileid: "72684456"
---
# <a name="tuple_element-class"></a>tuple_element 클래스

`tuple` 요소를 래핑합니다. 특수화는 `array` 요소 및 `pair` 요소를 래핑합니다.

## <a name="syntax"></a>구문

```cpp
// CLASS tuple_element (find element by index)
template <size_t Index, class Tuple>
   struct tuple_element;

// tuple_element for const
template <size_t Index, class Tuple>
   struct tuple_element<Index, const Tuple>;

// tuple_element for volatile
template <size_t Index, class Tuple>
   struct tuple_element<Index, volatile Tuple>;

// tuple_element for const volatile
template <size_t Index, class Tuple>
   struct tuple_element<Index, const volatile Tuple>;

// Helper typedef
template <size_t Index, class Tuple>
   using tuple_element_t = typename tuple_element<Index, Tuple>::type;

// Specialization for arrays
template <size_t Index, class Elem, size_t Size>
   struct tuple_element<Index, array<Elem, Size>>;

// Specializations for pairs
// struct to determine type of element 0 in pair
template <class T1, class T2>
   struct tuple_element<0, pair<T1, T2>>;

// struct to determine type of element 1 in pair
template <class T1, class T2>
   struct tuple_element<1, pair<T1, T2>>;
```

### <a name="parameters"></a>매개 변수

*인덱스* \
지정된 요소의 인덱스입니다.

*튜플* \
튜플의 형식입니다.

*Elem* \
배열 요소의 형식입니다.

*크기* \
배열의 크기입니다.

*T1* \
한 쌍의 첫 번째 요소 형식입니다.

*T2* \
쌍의 두 번째 요소 형식입니다.

## <a name="remarks"></a>주의

클래스 템플릿 `tuple_element`에는 튜플 형식 *튜플의*인덱스 *인덱스* 에 있는 형식에 대 한 동의어 인 중첩 된 typedef `type` 있습니다.

`tuple_element_t` 형식 정의는 `tuple_element<Index, Tuple>::type`에 사용할 수 있는 편리한 별칭입니다.

배열의 클래스 템플릿 특수화는 `array`에 대 한 인터페이스를 각각 동일한 형식을 갖는 `Size` 요소의 튜플로 제공 합니다. 각 특수화에는 `array`의 *Index* 요소 형식에 대 한 동의어 인 중첩 된 typedef `type` 있으며, 모든 const 휘발성 한정자가 유지 됩니다.

`pair` 형식의 템플릿 특수화는 각각 단일 구성원 형식 정의 `type`를 제공합니다. 이 형식 정의는 쌍의 지정된 위치에 있는 요소 형식과 동일한 의미이며, 모든 const 및/또는 volatile 한정자가 유지됩니다. `tuple_element_t` 형식 정의는 `tuple_element<N, pair<T1, T2>>::type`에 사용할 수 있는 편리한 별칭입니다.

[Get 함수 &lt;utility &gt;](../standard-library/utility-functions.md#get) 를 사용 하 여 지정 된 위치 또는 지정 된 형식의 요소를 반환할 수 있습니다.

## <a name="example"></a>예제

```cpp
#include <tuple>
#include <string>
#include <iostream>

using namespace std;
typedef tuple<int, double, string> MyTuple;

int main() {
    MyTuple c0{ 0, 1.5, "Tail" };

    tuple_element_t<0, MyTuple> val = get<0>(c0); //get by index
    tuple_element_t<1, MyTuple> val2 = get<1>(c0);
    tuple_element_t<2, MyTuple> val3 = get<string>(c0); // get by type

    cout << val << " " << val2 << " " << val3 << endl;
}
```

```Output
0 1.5 Tail
```

## <a name="example"></a>예제

```cpp
#include <array>
#include <iostream>

using namespace std;
typedef array<int, 4> MyArray;

int main()
{
    MyArray c0 { 0, 1, 2, 3 };

    for (const auto& e : c0)
    {
        cout << e << " ";
    }
    cout << endl;

    // display first element "0"
    tuple_element<0, MyArray>::type val = c0.front();
    cout << val << endl;
}
```

```Output
0 1 2 3
0
```

## <a name="example"></a>예제

```cpp
#include <utility>
#include <iostream>

using namespace std;

typedef pair<int, double> MyPair;
int main() {
    MyPair c0(0, 1.333);

    // display contents "0 1"
    cout << get<0>(c0) << " ";
    cout << get<1>(c0) << endl;

    // display first element "0 " by index
    tuple_element<0, MyPair>::type val = get<0>(c0);
    cout << val << " ";

    // display second element by type
    tuple_element<1, MyPair>::type val2 = get<double>(c0);
    cout << val2 << endl;
}
```

```Output
0 1.333
0 1.333
```

## <a name="requirements"></a>요구 사항

**헤더:** \<tuple>

**헤더:** \<array>(배열 특수화용)

**헤더:** \<utility > (쌍 특수화의 경우)

**네임스페이스:** std
