---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 133c394777dd3297def76a81b7d4cf9f628beccd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308918"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFill = new WorkbookRangeFill
{
    Color = "#FF0000"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["Sheet1"]
    .Range("$A$1").Format.Fill
    .Request()
    .UpdateAsync(workbookRangeFill);

```