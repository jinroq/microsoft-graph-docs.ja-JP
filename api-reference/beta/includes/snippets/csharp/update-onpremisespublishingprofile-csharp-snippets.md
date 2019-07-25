---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d7d523a61ff02af89e8171b6405e326f798b9c73
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878288"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var hybridAgentUpdaterConfiguration = new HybridAgentUpdaterConfiguration
{
    AllowUpdateConfigurationOverride = false
};

var onPremisesPublishingProfiles = new OnPremisesPublishingProfile();
onPremisesPublishingProfiles.HybridAgentUpdaterConfiguration = hybridAgentUpdaterConfiguration;

await graphClient.OnPremisesPublishingProfiles["provisioning"]
    .Request()
    .UpdateAsync(onPremisesPublishingProfiles);

```