---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b5b4312c65a8a42db6c33d9728a1bf84f7e99bc6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728414"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleSettings = await graphClient.PrivilegedRoles["{id}"].Settings
    .Request()
    .GetAsync();

```