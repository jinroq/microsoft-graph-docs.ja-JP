---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 85e8d6d2ee9af69447ad0ee8e7c86f0bb0c600bf
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36358560"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerDeviceUsageDistributionUserCounts = await graphClient.Reports
    .GetYammerDeviceUsageDistributionUserCounts("D7")
    .Request()
    .GetAsync();

```