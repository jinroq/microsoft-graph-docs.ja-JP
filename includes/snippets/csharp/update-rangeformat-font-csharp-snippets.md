---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e673e1326ddc235699d5664e91e8027d385690e0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737096"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = new WorkbookRangeFont
{
    Bold = true,
    Color = "#4B180E",
    Size = 26
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["Sheet1"].Range('$A$1').Format.Font
    .Request()
    .UpdateAsync(workbookRangeFont);

```