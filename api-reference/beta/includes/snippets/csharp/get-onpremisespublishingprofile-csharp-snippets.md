---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 126e6c5acc360b809e71b18b30fdc92cf1b66c7d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878443"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onPremisesPublishingProfile = await graphClient.OnPremisesPublishingProfiles["provisioning"]
    .Request()
    .Expand("agentGroups")
    .GetAsync();

```