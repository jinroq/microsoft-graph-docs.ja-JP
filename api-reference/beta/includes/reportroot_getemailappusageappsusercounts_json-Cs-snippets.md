---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f38fba43a737624e01894c25db015407301aeedc
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442334"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailAppUsageAppsUserCounts = await graphClient.Reports.GetEmailAppUsageAppsUserCounts('D7')
    .Request()
    .GetAsync();

```