---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bfa0e9990f87f0b1bdeddda9aa8ea8d1dfd047e6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471290"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetYammerDeviceUsageDistributionUserCounts('D7')
    .Request()
    .GetAsync();

```