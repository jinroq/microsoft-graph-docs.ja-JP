---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6c05834528bf98f5514b306ec7a4a1474b6749a2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460974"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var items = await graphClient.Drive.Items["{item-id}"]
    .Request()
    .Select( e => new {
             e.Content 
             })
    .GetAsync();

var content = items.Content;

```