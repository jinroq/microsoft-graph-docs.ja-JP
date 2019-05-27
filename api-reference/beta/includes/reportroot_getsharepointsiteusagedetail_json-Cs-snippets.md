---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7ed6c599a08a2314acf66c39be8e567df20176ee
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34464928"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSharePointSiteUsageDetail = await graphClient.Reports.GetSharePointSiteUsageDetail('D7')
    .Request()
    .GetAsync();

```