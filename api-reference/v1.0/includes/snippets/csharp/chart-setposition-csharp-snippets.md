---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: de7c2feea618ecf6f3d8b86eb357d3282e4e03e2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471574"
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