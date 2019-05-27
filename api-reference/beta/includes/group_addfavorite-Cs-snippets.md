---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f953d9ad67ca4558856cef72c7b961b5c9fe027d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444896"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"]
    .AddFavorite()
    .Request()
    .PostAsync();

```