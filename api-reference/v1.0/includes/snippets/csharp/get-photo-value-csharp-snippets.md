---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fcde4b8ff38a06313b1e8adfe9ac0c199bb1d416
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733378"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var Stream = await graphClient.Users["{id|userPrincipalName}"].Photo.Content
    .Request()
    .GetAsync();

```