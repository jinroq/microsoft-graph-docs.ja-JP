---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c420b6545366bac36d8eeae437b2a057ce4cc4bd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859858"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = new EducationUser();
educationUser.displayName = "Rogelio Cazares";
educationUser.givenName = "Rogelio";
educationUser.middleName = "Fernando";
educationUser.surname = "Cazares";

graphClient.education().users("13020")
    .buildRequest()
    .patch(educationUser);

```