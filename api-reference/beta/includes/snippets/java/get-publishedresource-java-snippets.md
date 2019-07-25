---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b977e6db9eff562540a5f761b9f70a332df836bc
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875184"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PublishedResource publishedResource = graphClient.onPremisesPublishingProfiles("provisioning").publishedResources("aed0b780-965f-4149-85c5-a8c73e58b67d")
    .buildRequest()
    .expand("agentGroups")
    .get();

```