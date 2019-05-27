---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cd3a8bb10ab477afd9f19f7b7195794ca9a343dd
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34482137"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{id}"].Workbook.Tables["{id|name}"].Columns["{id|name}"]
    .DataBodyRange()
    .Request()
    .PostAsync();

```