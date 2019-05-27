---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 18c4f891eb70cf857709f92567241045300abc1a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34468655"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var items = await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items
    .Request()
    .GetAsync();

```