---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 510ad31949da3e4bb6b29a020083dcd2fd3cd90c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449231"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var jobs = await graphClient.ServicePrincipals["{id}"].Synchronization.Jobs
    .Request()
    .GetAsync();

```