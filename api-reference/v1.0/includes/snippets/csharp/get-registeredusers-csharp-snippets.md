---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0dc71b6cb192b5faef6296aed191ea9590a3cab5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723470"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var registeredUsers = await graphClient.Devices["{id}"].RegisteredUsers
    .Request()
    .GetAsync();

```