---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6f46fb1c3f3ca66dc0938e9c925746170bdc9a0d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34468079"
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

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{sheet-id}"].Range('$C$1').Format
    .Request()
    .UpdateAsync(workbookRangeFormat);

```