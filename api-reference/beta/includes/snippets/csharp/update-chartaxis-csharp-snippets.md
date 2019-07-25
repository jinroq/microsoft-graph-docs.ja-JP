---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0e60d1d547ea8bbf50615c0cf7b907d3142e14a7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708357"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChartAxis = new WorkbookChartAxis
{
    MajorUnit = new Json
    {
    },
    Maximum = new Json
    {
    },
    Minimum = new Json
    {
    }
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"].Axes.ValueAxis
    .Request()
    .UpdateAsync(workbookChartAxis);

```