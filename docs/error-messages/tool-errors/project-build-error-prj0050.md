---
title: 프로젝트 빌드 오류 PRJ0050
ms.date: 11/04/2016
f1_keywords:
- PRJ0050
helpviewer_keywords:
- PRJ0050
ms.assetid: ceef3b37-0acf-4abd-ac62-aa830b4fa145
ms.openlocfilehash: 56e092b5f7c33ad9543951621b2a9d8f6992331f
ms.sourcegitcommit: 857fa6b530224fa6c18675138043aba9aa0619fb
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/24/2020
ms.locfileid: "80191992"
---
# <a name="project-build-error-prj0050"></a>프로젝트 빌드 오류 PRJ0050

출력을 등록하지 못했습니다. 레지스트리를 수정할 수 있는 적절 한 권한이 있는지 확인 하세요.

Visual C++ build system에서 빌드 (dll 또는 .exe)의 출력을 등록할 수 없습니다. 레지스트리를 수정 하려면 관리자로 로그온 해야 합니다.

.Dll을 빌드하는 경우에는 shutdown.exe를 사용 하 여 .dll을 수동으로 등록할 수 있습니다. 이렇게 하면 빌드에 실패 한 이유에 대 한 정보가 표시 됩니다.

.Dll을 빌드하지 않는 경우 오류를 발생 시키는 명령에 대 한 빌드 로그를 확인 합니다.
