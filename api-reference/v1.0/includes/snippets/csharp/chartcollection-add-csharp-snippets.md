---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0b5739ae3ab82a5a0e90636205ce2fc12f66cea6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735720"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "ColumnStacked";

var sourceData = "A1:B1";

var seriesBy = "Auto";

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts
    .Add(type,sourceData,seriesBy)
    .Request()
    .PostAsync();

```