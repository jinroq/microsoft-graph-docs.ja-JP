---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 469c0ce2e847181b58b3205b6209724fa5d1a066
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441956"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getMailboxUsageQuotaStatusMailboxCounts = await graphClient.Reports.GetMailboxUsageQuotaStatusMailboxCounts('D7')
    .Request()
    .GetAsync();

```