---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a1409e2e4219de38ef33d7ebbf0a552b42390a6e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526174"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerDeviceUsageDistributionUserCounts = await graphClient.Reports.GetYammerDeviceUsageDistributionUserCounts('D7')
    .Request()
    .GetAsync();

```