---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 83706e6c53bf56778ff6b9f9a37a635577d4ef15
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721186"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var oAuth2PermissionGrant = new OAuth2PermissionGrant
{
    Scope = "scope-value"
};

await graphClient.OAuth2Permissiongrants["{id}"]
    .Request()
    .UpdateAsync(oAuth2PermissionGrant);

```