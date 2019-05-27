---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ec741e1211d495cab88e0e29a2f370e50eb9c882
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34464771"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointSiteUsageSiteCounts = await graphClient.Reports.GetSharePointSiteUsageSiteCounts('D7')
    .Request()
    .GetAsync();

```