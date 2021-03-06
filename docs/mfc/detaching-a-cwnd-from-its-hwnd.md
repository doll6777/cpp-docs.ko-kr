---
title: CWnd를 해당 HWND에서 분리
ms.date: 11/04/2016
helpviewer_keywords:
- HWND, detaching CWnd from
- removing HWNDs from CWnds
- CWnd objects [MFC], detaching from HWND
- detaching CWnds from HWNDs
- Detach method (CWnd class)
ms.assetid: 6efadf84-0517-4a3f-acfd-216e088f19c6
ms.openlocfilehash: 2e0484698654cd14f22a92be76a80f71c0f9adf5
ms.sourcegitcommit: c21b05042debc97d14875e019ee9d698691ffc0b
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 06/09/2020
ms.locfileid: "84621852"
---
# <a name="detaching-a-cwnd-from-its-hwnd"></a>CWnd를 해당 HWND에서 분리

개체 관계를 회피 해야 하는 경우 `HWND` MFC는 `CWnd` Windows 창에서 c + + 창 개체와의 연결을 끊는 또 다른 멤버 함수인 [Detach](reference/cwnd-class.md#detach)를 제공 합니다. 이렇게 하면 개체가 소멸 될 때 소멸자가 Windows 창을 소멸 시킬 수 없습니다.

## <a name="what-do-you-want-to-know-more-about"></a>자세히 알아야 할 내용

- [창 만들기](creating-windows.md)

- [창 소멸 시퀀스](window-destruction-sequence.md)

- [창 메모리 할당 및 할당 취소](allocating-and-deallocating-window-memory.md)

## <a name="see-also"></a>참고 항목

[창 개체](window-objects.md)
