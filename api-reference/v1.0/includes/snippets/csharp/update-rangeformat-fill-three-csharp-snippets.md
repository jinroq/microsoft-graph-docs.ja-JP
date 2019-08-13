---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9bdc9fac6de8ec400d333568b8d6f8c3a449c4a3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324825"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFill = new WorkbookRangeFill
{
    Color = "#0000FF"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{sheet-id}"]
    .Range("$C$1").Format.Fill
    .Request()
    .UpdateAsync(workbookRangeFill);

```