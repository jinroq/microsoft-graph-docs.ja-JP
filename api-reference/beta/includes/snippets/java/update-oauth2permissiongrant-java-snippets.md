---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e89d3aad5d4ce92c105c001750a404d426f648a3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878935"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OAuth2PermissionGrant oAuth2PermissionGrant = new OAuth2PermissionGrant();
oAuth2PermissionGrant.scope = "scope-value";

graphClient.oAuth2Permissiongrants("{id}")
    .buildRequest()
    .patch(oAuth2PermissionGrant);

```