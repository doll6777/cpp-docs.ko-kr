---
title: 컴파일러 오류 C3824
ms.date: 11/04/2016
f1_keywords:
- C3824
helpviewer_keywords:
- C3824
ms.assetid: b6c6adf1-0a29-401c-a06e-616fd50d4c37
ms.openlocfilehash: 78081de44a834b16d34d1f88a5dc996efb1f784c
ms.sourcegitcommit: 1f009ab0f2cc4a177f2d1353d5a38f164612bdb1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/27/2020
ms.locfileid: "87220147"
---
# <a name="compiler-error-c3824"></a>컴파일러 오류 C3824

' member ':이 형식은이 컨텍스트 (함수 매개 변수, 반환 형식 또는 정적 멤버)에 사용할 수 없습니다.

고정 포인터는 함수 매개 변수, 반환 형식 또는 선언할 수 없습니다 **`static`** .

## <a name="example"></a>예제

다음 샘플에서는 C3824를 생성 합니다.

```cpp
// C3824a.cpp
// compile with: /clr /c
void func() {
   static pin_ptr<int> a; // C3824
   pin_ptr<int> b; // OK
}
```
