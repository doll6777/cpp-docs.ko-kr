---
title: 컴파일러 오류 C3711
ms.date: 11/04/2016
f1_keywords:
- C3711
helpviewer_keywords:
- C3711
ms.assetid: 26d581cc-2153-4ee0-b814-a371184be3e1
ms.openlocfilehash: bf8d1ea745ed96d782fdc95d825e278e894066ef
ms.sourcegitcommit: 1f009ab0f2cc4a177f2d1353d5a38f164612bdb1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/27/2020
ms.locfileid: "87220186"
---
# <a name="compiler-error-c3711"></a>컴파일러 오류 C3711

' method ': 관리 되지 않는 이벤트 소스 메서드는 void 또는 정수 계열 형식을 반환 해야 합니다.

Void 또는 정수 계열 형식을 반환 하지 않는 메서드를 이벤트 소스에서 정의 했습니다. 이 오류를 해결 하려면 이벤트 및 이벤트 처리기의 반환 형식이 또는 **`void`** 와 같은 정수 계열 형식 인지 확인 합니다 **`int`** **`long`** .

다음 샘플에서는 C3711를 생성 합니다.

```cpp
// C3711.cpp
#include <atlbase.h>
#include <atlcom.h>
#include <atlctl.h>

[event_source(native)]
class CEventSrc {
public:
   __event float event1();   // C3711
   // try the following line instead
   // __event int event1();
   // also change the handler, below
};

[event_receiver(native)]
class CEventRec {
public:
   float handler1() {         // change float to int
      return 0.0;             // change 0.0 to 0
   }
   void HookEvents(CEventSrc* pSrc) {
      __hook(CEventSrc::event1, pSrc, CEventRec::handler1);
   }
   void UnhookEvents(CEventSrc* pSrc) {
      __unhook(CEventSrc::event1, pSrc, CEventRec::handler1);
   }
};

int main() {
}
```
