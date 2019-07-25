---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8a5ef2f86b1713799a0a590611c87d88724925d9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878567"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onPremisesAgentGroup = await graphClient.OnPremisesPublishingProfiles["provisioning"].AgentGroups["2d55ed41-1619-4848-92bb-0576d3038682"]
    .Request()
    .Expand("agents")
    .GetAsync();

```