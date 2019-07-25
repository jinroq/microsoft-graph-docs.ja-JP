---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2c129dbb0dd445a746cab840ebf5eaf838ded49c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878476"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agentGroups = await graphClient.OnPremisesPublishingProfiles["provisioning"].AgentGroups
    .Request()
    .Expand("publishedResources")
    .GetAsync();

```