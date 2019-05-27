---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ff80ff9b4fb36607e2bf97d3d1c9f8842cbb79d7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34481255"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subscription = await graphClient.Subscriptions["{id}"]
    .Request()
    .GetAsync();

```