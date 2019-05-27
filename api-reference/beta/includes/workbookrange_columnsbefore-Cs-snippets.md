---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8d578ef84b324ecb5453c3c418734fe51431258f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34478581"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drive.Root.Workbook.Worksheets["{id}"]
    .Range()
    .ColumnsBefore(count)
    .Request()
    .PostAsync();

```