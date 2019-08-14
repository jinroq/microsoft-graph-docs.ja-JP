---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 79b8248558242d401b6abfc5862ce0f1dd0726c0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372749"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = new WorkbookRangeFont
{
    Italic = true,
    Size = 26
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["Sheet1"]
    .Range("$B$1").Format.Font
    .Request()
    .UpdateAsync(workbookRangeFont);

```