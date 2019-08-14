---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e9f3050a0f8d8e070b2536ce0ccb0c38c056e12b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372757"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFormat = new WorkbookRangeFormat
{
    ColumnWidth = 135,
    HorizontalAlignment = "Right",
    VerticalAlignment = "Top",
    RowHeight = 49,
    WrapText = false
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["Sheet1"]
    .Range("$C$1").Format
    .Request()
    .UpdateAsync(workbookRangeFormat);

```