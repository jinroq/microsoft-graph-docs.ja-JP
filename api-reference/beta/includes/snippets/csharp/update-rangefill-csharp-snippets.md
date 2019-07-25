---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ed829c50c571add47f1836b4dd1fb6efe2d920b9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35874546"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFill = new WorkbookRangeFill
{
    Color = "color-value"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range().Format.Fill
    .Request()
    .UpdateAsync(workbookRangeFill);

```