---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 23ec53bdc5b18bb28dd434064892da3b8b02723c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707867"
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