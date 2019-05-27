---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: efcc5891d38122349b5e233428bb6a614011b260
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440941"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveUsageFileCounts = await graphClient.Reports.GetOneDriveUsageFileCounts('D7')
    .Request()
    .GetAsync();

```