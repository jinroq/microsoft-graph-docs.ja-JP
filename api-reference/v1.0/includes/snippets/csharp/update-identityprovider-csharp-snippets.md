---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9912355f20a6ba80374f022bb3e055ecf6e274b0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35513888"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProvider = new IdentityProvider
{
    ClientSecret = "1111111111111"
};

await graphClient.IdentityProviders["Amazon-OAuth"]
    .Request()
    .UpdateAsync(identityProvider);

```