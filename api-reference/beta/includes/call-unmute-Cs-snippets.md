---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c1f77c5ea2102b0cc5ae408aa8f92dd05a4a1365
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34456145"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "clientContext-value";

await graphClient.App.Calls["{id}"]
    .Unmute(clientContext)
    .Request()
    .PostAsync();

```