---
title: 컴파일러 오류 C3012
ms.date: 11/04/2016
f1_keywords:
- C3012
helpviewer_keywords:
- C3012
ms.assetid: cc7040b1-b3fb-4da6-a474-877914d30332
ms.openlocfilehash: 69f0544815804e9827631be81bf9735a95bd1a22
ms.sourcegitcommit: 857fa6b530224fa6c18675138043aba9aa0619fb
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/24/2020
ms.locfileid: "80176704"
---
# <a name="compiler-error-c3012"></a>컴파일러 오류 C3012

> '*내장*함수 ': 병렬 영역 내부에서는 직접 내장 함수를 사용할 수 없습니다.

[컴파일러 내장](../../intrinsics/compiler-intrinsics.md) 함수는 `omp parallel` 지역에서 사용할 수 없습니다. 이 문제를 해결 하려면 내장 함수를 지역 외부로 이동 하거나 비 내장 함수로 바꿉니다.

## <a name="example"></a>예제

다음 샘플에서는 C3012를 생성 하 고이를 해결 하는 한 가지 방법을 보여 줍니다.

```cpp
// C3012.cpp
// compile with: /openmp
#ifdef __cplusplus
extern "C" {
#endif
void* _ReturnAddress();
#ifdef __cplusplus
}
#endif

int main()
{
   #pragma omp parallel
   {
      _ReturnAddress();   // C3012
   }
   _ReturnAddress();      // OK
}
```
