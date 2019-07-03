---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: eaaa002278b2b7e45e9bf60b35e634a0624dd4de
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486847"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFill = new WorkbookRangeFill
{
    Color = "color-value"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"].Range().Format.Fill
    .Request()
    .UpdateAsync(workbookRangeFill);

```