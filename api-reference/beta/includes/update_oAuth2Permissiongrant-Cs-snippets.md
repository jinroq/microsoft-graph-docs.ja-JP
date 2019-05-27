---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 83706e6c53bf56778ff6b9f9a37a635577d4ef15
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34476551"
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