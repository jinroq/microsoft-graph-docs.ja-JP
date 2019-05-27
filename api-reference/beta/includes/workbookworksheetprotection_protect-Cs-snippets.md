---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 650f253ed5663d1a117c0878744c33160cf5dba7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34453125"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var options = new WorkbookWorksheetProtectionOptions
{
    AllowFormatCells = true,
    AllowFormatColumns = true,
    AllowFormatRows = true,
    AllowInsertColumns = true,
    AllowInsertRows = true,
    AllowInsertHyperlinks = true,
    AllowDeleteColumns = true,
    AllowDeleteRows = true,
    AllowSort = true,
    AllowAutoFilter = true,
    AllowPivotTables = true
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Protection
    .Protect(options)
    .Request()
    .PostAsync();

```