---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ec1e3b02899db809f8d4a8a14d1623f1e19f0593
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442768"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var across = true;

await graphClient.Me.Drive.Items["{id}"].Workbook.Names["{name}"]
    .Range()
    .Merge(across)
    .Request()
    .PostAsync();

```