---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3e22caa17cc852afbdf8745577ac9cfd4c282297
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708256"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartDataLabels = new WorkbookChartDataLabels
{
    Position = "position-value",
    ShowValue = true,
    ShowSeriesName = true,
    ShowCategoryName = true,
    ShowLegendKey = true
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].DataLabels
    .Request()
    .UpdateAsync(workbookChartDataLabels);

```