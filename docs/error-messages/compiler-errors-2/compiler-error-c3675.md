---
title: 컴파일러 오류 C3675
ms.date: 11/04/2016
f1_keywords:
- C3675
helpviewer_keywords:
- C3675
ms.assetid: 87461613-6633-430b-b95d-c7cb1bb63776
ms.openlocfilehash: 6772572d29765370d6cdbf52ed8470ff2f3f054e
ms.sourcegitcommit: 16fa847794b60bf40c67d20f74751a67fccb602e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/03/2019
ms.locfileid: "74758075"
---
# <a name="compiler-error-c3675"></a>컴파일러 오류 C3675

' function ': ' property '가 정의 되어 있으므로 예약 되어 있습니다.

간단한 속성을 선언 하는 경우 컴파일러는 get 및 set 접근자 메서드를 생성 하 고 이러한 이름은 프로그램의 범위에 표시 됩니다.  컴파일러에서 생성 된 이름은 get_ 앞에, 속성 이름에 set_ 하 여 구성 됩니다.  따라서 컴파일러에서 생성 된 접근자와 동일한 이름을 가진 함수를 선언할 수 없습니다.

자세한 내용은 [property](../../extensions/property-cpp-component-extensions.md) 를 참조하세요.

## <a name="example"></a>예제

다음 샘플에서는 C3675를 생성 합니다.

```cpp
// C3675.cpp
// compile with: /clr /c
ref struct C {
public:
   property int Size;
   int get_Size() { return 0; }   // C3675
};
```
