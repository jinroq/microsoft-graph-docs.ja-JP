---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d1d4212611a535f0d014a6fc7f6bf6c7cf2bb935
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442166"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailAppUsageVersionsUserCounts = await graphClient.Reports.GetEmailAppUsageVersionsUserCounts('D7')
    .Request()
    .GetAsync();

```