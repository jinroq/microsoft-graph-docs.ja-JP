---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9c5aca27fa617fe465b2eb63e14635906f807203
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34456250"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "clientContext-value";

await graphClient.App.Calls["{id}"]
    .Mute(clientContext)
    .Request()
    .PostAsync();

```