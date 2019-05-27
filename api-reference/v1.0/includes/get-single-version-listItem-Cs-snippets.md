---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a75cfb7a7b002adc388e7a02b2953ea5dd58f478
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462477"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var listItemVersion = await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{item-id}"].Versions["{version-id}"]
    .Request()
    .GetAsync();

```