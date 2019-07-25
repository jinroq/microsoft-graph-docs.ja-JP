---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cdc1ab8ee0802c964e914738a1c64b758c80fa94
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869277"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var criteria = new SynchronizationJobRestartCriteria
{
    ResetScope = SynchronizationJobRestartScope.QuarantineState | SynchronizationJobRestartScope.Watermark | SynchronizationJobRestartScope.Escrows
};

await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs["{jobId}"]
    .Restart(criteria)
    .Request()
    .Header("Authorization","Bearer <token>")
    .PostAsync();

```