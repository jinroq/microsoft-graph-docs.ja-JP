---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4aa38df46556e2a16ca3100b126e5a0512b38005
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875040"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PublishedResource publishedResource = new PublishedResource();
publishedResource.displayName = "New provisioning";
publishedResource.resourceName = "domain1.contoso.com";

graphClient.onPremisesPublishingProfiles("provisioning").publishedResources()
    .buildRequest()
    .post(publishedResource);

```