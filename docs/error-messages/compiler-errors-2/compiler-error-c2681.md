---
title: 컴파일러 오류 C2681
ms.date: 11/04/2016
f1_keywords:
- C2681
helpviewer_keywords:
- C2681
ms.assetid: eb42da6d-8d2c-43fd-986b-e73e2b004885
ms.openlocfilehash: d7cf39e89f70f27471fb3a251aac12793f1fb33b
ms.sourcegitcommit: 16fa847794b60bf40c67d20f74751a67fccb602e
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/03/2019
ms.locfileid: "74760298"
---
# <a name="compiler-error-c2681"></a>컴파일러 오류 C2681

' type ': 이름에 대 한 식 형식이 잘못 되었습니다.

캐스팅 연산자가 잘못 된 형식에서 변환 하려고 했습니다. 예를 들어 [dynamic_cast](../../cpp/dynamic-cast-operator.md) 연산자를 사용 하 여 식을 포인터 형식으로 변환 하는 경우 소스 식은 포인터 여야 합니다.

다음 샘플에서는 C2681를 생성 합니다.

```cpp
// C2681.cpp
class A { virtual void f(); };

void g(int i) {
    A* pa;
    pa = dynamic_cast<A*>(i);  // C2681
}
```
