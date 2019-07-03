---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 71852acab78ed19439969ba52fcf9848c1fb29b7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526331"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const groupLifecyclePolicy = {
  groupLifetimeInDays: 100,
  managedGroupTypes: "Selected",
  alternateNotificationEmails: "admin@contoso.com"
};

let res = await client.api('/groupLifecyclePolicies')
    .version('beta')
    .post({groupLifecyclePolicy : groupLifecyclePolicy});

```