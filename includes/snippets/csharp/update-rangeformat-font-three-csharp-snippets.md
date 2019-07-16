---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 96c8f12df4cdf664046764476ec4cd1646d1c3e9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737116"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = new WorkbookRangeFont
{
    Underline = "Single",
    Color = "#FFFFFF",
    Size = 26
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["Sheet1"].Range('$C$1').Format.Font
    .Request()
    .UpdateAsync(workbookRangeFont);

```