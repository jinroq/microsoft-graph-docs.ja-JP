---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 225dc419576d2658567bea450d2aa070d0b2c515
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736666"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sourceData = "sourceData-value";

var seriesBy = "seriesBy-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"]
    .SetData(sourceData,seriesBy)
    .Request()
    .PostAsync();

```