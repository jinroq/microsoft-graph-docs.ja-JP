---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3fbc6055660aa3c9e21fc6c7e0a71ec20ef8ed34
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710095"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const appRoleAssignment = {
  creationTimestamp: "2016-10-19T10:37:00Z",
  principalDisplayName: "principalDisplayName-value",
  principalId: "principalId-value",
  principalType: "principalType-value",
  resourceDisplayName: "resourceDisplayName-value"
};

let res = await client.api('/appRoleAssignments/{id}')
    .version('beta')
    .update({appRoleAssignment : appRoleAssignment});

```