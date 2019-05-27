---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a7ec8819005c21715473378fe105484d3c0f26e6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447909"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var people = await graphClient.Me.People
    .Request()
    .GetAsync();

```