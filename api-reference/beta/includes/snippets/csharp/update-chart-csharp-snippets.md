---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 749ecae73c2aeba28b2234705fa4a153b034721c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708441"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookChart = new WorkbookChart
{
    Height = 99,
    Left = 99
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"]
    .Request()
    .UpdateAsync(workbookChart);

```