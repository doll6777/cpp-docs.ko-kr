---
title: 프로젝트 빌드 오류 PRJ0032
ms.date: 11/04/2016
f1_keywords:
- PRJ0032
helpviewer_keywords:
- PRJ0032
ms.assetid: bc6acbea-4041-4237-8b5a-f0434705d89f
ms.openlocfilehash: 62efa0e72c6fbe4bd38983ff0507923392427c04
ms.sourcegitcommit: 857fa6b530224fa6c18675138043aba9aa0619fb
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/24/2020
ms.locfileid: "80192486"
---
# <a name="project-build-error-prj0032"></a>프로젝트 빌드 오류 PRJ0032

프로젝트 수준 사용자 지정 빌드 단계의 ' 출력 ' 속성에 ' s t r u e '가 포함 되어 ' macro_expansion '로 계산 됩니다.

프로젝트에 대 한 사용자 지정 빌드 단계는 매크로 평가 문제로 인해 잘못 된 출력이 있습니다. 이 오류는 경로 형식이 잘못 된 것을 의미할 수도 있습니다 .이 경우 파일 경로에 잘못 된 문자 또는 문자 조합이 포함 됩니다.

이 오류를 해결 하려면 매크로를 수정 하거나 경로 지정을 수정 합니다. 계산 된 경로는 프로젝트 디렉터리의 절대 경로입니다.
