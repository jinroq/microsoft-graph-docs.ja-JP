---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4f82cb90fcecd47d6f218a9d12b1dfa6a1908264
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436566"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Items["{item-id}"]
    .Follow()
    .Request()
    .PostAsync();

```