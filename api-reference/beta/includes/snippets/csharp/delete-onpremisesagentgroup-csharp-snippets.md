---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e7ac396c9294f671c3e03182f30bd41dab5e77c2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878530"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.OnPremisesPublishingProfiles["provisioning"].AgentGroups["8832388F-3814-4952-B288-FFB62081FE25"]
    .Request()
    .DeleteAsync();

```