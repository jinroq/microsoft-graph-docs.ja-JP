---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9912355f20a6ba80374f022bb3e055ecf6e274b0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705320"
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