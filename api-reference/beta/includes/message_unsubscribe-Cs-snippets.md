---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 35f5686cb351b5181c30b5d633b84e3c12404e74
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443930"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{id}"]
    .Unsubscribe()
    .Request()
    .PostAsync();

```