---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a113ed8c7b0d5a1e519b1b44e1b573d39c9741f5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720187"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const privilegedRoleAssignment = {
  reason: "reason-value",
  ticketNumber: "ticketNumber-value",
  ticketSystem: "ticketSystem-value"
};

let res = await client.api('/privilegedRoleAssignments/{id}/makePermanent')
    .version('beta')
    .post(privilegedRoleAssignment);

```