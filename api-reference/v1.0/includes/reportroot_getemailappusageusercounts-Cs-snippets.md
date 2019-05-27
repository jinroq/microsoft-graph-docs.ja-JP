---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7c94454b4ad6da695402a77eb69982195de1b62c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440619"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetEmailAppUsageUserCounts('D7')
    .Request()
    .GetAsync();

```