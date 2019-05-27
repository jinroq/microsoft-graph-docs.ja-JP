---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2959b6731cceca6353c3a0c160ed0881e20d36e2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447951"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ownedObjects = await graphClient.Me.OwnedObjects
    .Request()
    .GetAsync();

```