---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 23ec53bdc5b18bb28dd434064892da3b8b02723c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475396"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartSeries = new WorkbookChartSeries
{
    Name = "name-value"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Series["{undefined}"]
    .Request()
    .UpdateAsync(workbookChartSeries);

```