---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 99d1e3979aada0dd54301f464a472c358288abba
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736252"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = new WorkbookRangeFont
{
    Bold = true,
    Color = "color-value",
    Italic = true,
    Name = "name-value",
    Size = 99,
    Underline = "underline-value"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Format.Font
    .Request()
    .UpdateAsync(workbookRangeFont);

```