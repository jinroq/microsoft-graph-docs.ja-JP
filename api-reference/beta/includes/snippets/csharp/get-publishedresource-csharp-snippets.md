---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 12a307132a5849bcef71530338004827814a165a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875186"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var publishedResource = await graphClient.OnPremisesPublishingProfiles["provisioning"].PublishedResources["aed0b780-965f-4149-85c5-a8c73e58b67d"]
    .Request()
    .Expand("agentGroups")
    .GetAsync();

```