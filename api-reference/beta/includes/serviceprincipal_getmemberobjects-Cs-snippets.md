---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 15d6af9dbccdf54eed689579c46dc04a200be525
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469386"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.ServicePrincipals["{id}"]
    .GetMemberObjects(securityEnabledOnly)
    .Request()
    .PostAsync();

```