---
title: 리소스 식별자(기호) (C++)
ms.date: 02/14/2019
f1_keywords:
- vc.editors.symbol.identifiers
helpviewer_keywords:
- symbols [C++], resource identifiers
- symbols [C++], creating
- resource symbols
- symbols [C++], editing
- resource editors [C++], resource symbols
ms.assetid: 8fccc09a-0237-4a65-b9c4-57d60c59e324
ms.openlocfilehash: c6b3cf7d3edfc870164645632bb07bf49c792a48
ms.sourcegitcommit: c123cc76bb2b6c5cde6f4c425ece420ac733bf70
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/14/2020
ms.locfileid: "81359896"
---
# <a name="resource-identifiers-symbols-c"></a>리소스 식별자(기호) (C++)

기호는 두 부분으로 구성된 리소스 식별자(ID) 즉, 기호 값(정수)에 매핑된 기호 이름(텍스트 문자열)입니다.

```cpp
IDC_EDITNAME = 5100
```

기호 이름은 가장 흔히 식별자라고 합니다.

소스 코드와 리소스 편집기에서 기호를 사용하여 작업하는 동안 기호는 리소스 및 사용자 인터페이스 개체를 참조하는 방법에 대한 설명을 제공합니다. [리소스 기호 대화 상자](../windows/viewing-resource-symbols.md)를 사용하여 한곳에서 편안하게 기호를 보고 조작할 수 있습니다.

애플리케이션의 크기가 커지고 복잡해질수록 리소스와 기호 수도 증가합니다. 여러 파일에 흩어져 있는 많은 기호를 추적하는 작업은 어려울 수 있습니다. **리소스 기호** 대화 상자는 다음과 같은 중앙 도구를 제공하여 기호 관리를 단순화합니다.

- [기호 만들기](../windows/creating-new-symbols.md)

- [기호 관리](../windows/changing-a-symbol-or-symbol-name-id.md)

- [미리 정의된 기호 ID 보기](../windows/predefined-symbol-ids.md)

새 리소스 또는 리소스 개체를 만들 때 [리소스 편집기](../windows/resource-editors.md) 에서는 리소스에 기본 이름(예: `IDC_RADIO1`)을 지정하고 값을 할당합니다. 이름-값-값 정의 `Resource.h` 파일에 저장 됩니다.

> [!NOTE]
> .rc 파일 간에 리소스 또는 리소스 개체를 복사할 경우 Visual C++에서는 기존 파일에 있는 기호 이름 또는 값과의 충돌을 방지하려고 복사된 리소스의 기호 값 또는 기호 이름과 값을 변경할 수 있습니다.

## <a name="requirements"></a>요구 사항

Win32

## <a name="see-also"></a>참고 항목

[리소스 파일 작업](../windows/working-with-resource-files.md)<br/>
[리소스 파일](../windows/resource-files-visual-studio.md)<br/>
[리소스 편집기](../windows/resource-editors.md)<br/>
