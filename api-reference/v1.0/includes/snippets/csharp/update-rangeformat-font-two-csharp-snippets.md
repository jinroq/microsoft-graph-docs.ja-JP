---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d6ef410a71edab9a83dff0bfebb61c5ec86f690c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324812"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFont = new WorkbookRangeFont
{
    Italic = true,
    Size = 26
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{sheet-id}"]
    .Range("$B$1").Format.Font
    .Request()
    .UpdateAsync(workbookRangeFont);

```