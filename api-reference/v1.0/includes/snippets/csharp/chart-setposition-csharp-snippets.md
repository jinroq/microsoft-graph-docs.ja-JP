---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: de7c2feea618ecf6f3d8b86eb357d3282e4e03e2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723169"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var startCell = "startCell-value";

var endCell = "endCell-value";

await graphClient.Me.Drive.Items["{id}"].Workbook.Worksheets["{id|name}"].Charts["{name}"]
    .SetPosition(startCell,endCell)
    .Request()
    .PostAsync();

```