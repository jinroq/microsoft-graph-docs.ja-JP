---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 441546c9d3508201deaa97396ed4fcc6f25120a2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320549"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetTeamsDeviceUsageDistributionUserCounts("D7")
    .Request()
    .GetAsync();

```