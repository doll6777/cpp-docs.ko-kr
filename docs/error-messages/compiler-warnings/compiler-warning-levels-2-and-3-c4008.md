---
title: 컴파일러 경고(수준 2 및 3) C4008
ms.date: 11/04/2016
f1_keywords:
- C4008
helpviewer_keywords:
- C4008
ms.assetid: fb45e535-cb68-4743-80e9-a6e34cfffeca
ms.openlocfilehash: ab51b16331cc6a102c828234d2c2b8be84f2d276
ms.sourcegitcommit: 1f009ab0f2cc4a177f2d1353d5a38f164612bdb1
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/27/2020
ms.locfileid: "87225243"
---
# <a name="compiler-warning-levels-2-and-3-c4008"></a>컴파일러 경고(수준 2 및 3) C4008

'identifier': 'attribute' 특성이 무시됩니다.

컴파일러가 **`__fastcall`** **`static`** **`inline`** 함수 (수준 3 경고) 또는 데이터 (수준 2 경고)에 대 한, 또는 특성을 무시 했습니다.

### <a name="to-fix-by-checking-the-following-possible-causes"></a>다음과 같은 가능한 원인을 확인하여 수정하려면

1. **`__fastcall`** 데이터가 있는 특성입니다.

1. **`static`****`inline`** **main** 함수를 사용 하는 또는 특성입니다.
