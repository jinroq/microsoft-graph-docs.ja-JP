---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0d0bef54d066a5a8f8719dc6c957f2844d09cef8
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737830"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var workbookRangeFill = new WorkbookRangeFill
{
    Color = "#00FF00"
};

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{sheet-id}"].Range('$B$1').Format.Fill
    .Request()
    .UpdateAsync(workbookRangeFill);

```