---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1b6b84552d6322a00b76ba32b2bf7d4d38b7020a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878427"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnPremisesPublishingProfile onPremisesPublishingProfile = graphClient.onPremisesPublishingProfiles("provisioning")
    .buildRequest()
    .expand("agentGroups")
    .get();

```