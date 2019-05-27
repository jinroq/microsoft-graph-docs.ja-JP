---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 65bc190f85fab212ecdebf1f6aa3444f64c88588
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34478266"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var worksheets = await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets
    .Request()
    .GetAsync();

```