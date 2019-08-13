---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8e6f1e2a44cca3b80df3bfc2ccdf18c9b203f333
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324818"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFill = new WorkbookRangeFill
{
    Color = "#FF0000"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{sheet-id}"]
    .Range("$A$1").Format.Fill
    .Request()
    .UpdateAsync(workbookRangeFill);

```