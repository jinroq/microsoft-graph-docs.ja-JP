---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5a4787b9c0e0e3c395f55e1d980174f20e18ffef
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737248"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartGridlines = new WorkbookChartGridlines
{
    Visible = true
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Axes.ValueAxis.MinorGridlines
    .Request()
    .UpdateAsync(workbookChartGridlines);

```