---
title: 프로젝트 빌드 오류 PRJ0025
ms.date: 08/27/2018
f1_keywords:
- PRJ0025
helpviewer_keywords:
- PRJ0025
ms.assetid: 57725c78-bc63-44f3-9667-2969b2d7c41d
ms.openlocfilehash: 30445a3abc2a6ad05c983448f57ed5b93df6e61f
ms.sourcegitcommit: 857fa6b530224fa6c18675138043aba9aa0619fb
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/24/2020
ms.locfileid: "80192356"
---
# <a name="project-build-error-prj0025"></a>프로젝트 빌드 오류 PRJ0025

> '*File*' 배치 파일에 사용자의 ANSI 코드 페이지로 변환할 수 없는 유니코드 내용이 포함 되어 있습니다.
>
> *파일의 유니코드 내용*

프로젝트 시스템에서 사용자의 현재 ANSI 코드 페이지로 제대로 변환할 수 없는 사용자 지정 빌드 규칙 또는 빌드 이벤트의 유니코드 내용을 찾았습니다.

이 오류에 대 한 해결 방법은 ANSI를 사용 하도록 빌드 규칙 또는 빌드 이벤트의 콘텐츠를 업데이트 하 고, 컴퓨터에 코드 페이지를 설치 하 고 시스템 기본값으로 설정 하는 것입니다.

사용자 지정 빌드 단계 및 빌드 이벤트에 대 한 자세한 내용은 [사용자 지정 빌드 단계 및 빌드 이벤트 이해](../../build/understanding-custom-build-steps-and-build-events.md)를 참조 하세요.
