---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7002995c98e7b918f04422a82703906c85958c74
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725233"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const servicePrincipal = {
  accountEnabled: true,
  addIns: [
    {
      id: "id-value",
      type: "type-value",
      properties: [
        {
          key: "key-value",
          value: "value-value"
        }
      ]
    }
  ],
  appDisplayName: "appDisplayName-value",
  appId: "appId-value",
  appOwnerOrganizationId: "appOwnerOrganizationId-value",
  appRoleAssignmentRequired: true
};

let res = await client.api('/servicePrincipals/{id}')
    .version('beta')
    .update({servicePrincipal : servicePrincipal});

```