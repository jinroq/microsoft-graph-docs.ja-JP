---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7c43f159d08f51132d889bf09c1ee7c222d4d71c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737095"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFormat = new WorkbookRangeFormat
{
    ColumnWidth = 135,
    HorizontalAlignment = "Center",
    VerticalAlignment = "Center",
    RowHeight = 49,
    WrapText = false
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["Sheet1"].Range('$B$1').Format
    .Request()
    .UpdateAsync(workbookRangeFormat);

```