---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b6b353d82ea072ad6b6680bd9cc0b34e3cbafac5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705298"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviders = await graphClient.IdentityProviders
    .Request()
    .GetAsync();

```