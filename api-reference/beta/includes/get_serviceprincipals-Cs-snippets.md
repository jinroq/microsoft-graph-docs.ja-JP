---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ef8b711a2f7bee18c4d2c1c4a0eda0cd94c77477
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446177"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipals = await graphClient.ServicePrincipals
    .Request()
    .GetAsync();

```