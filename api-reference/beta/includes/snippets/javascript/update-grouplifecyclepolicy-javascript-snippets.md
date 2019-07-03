---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b87c8b4e56d51f886cc1efd1a3f03df52f0dfd57
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35464559"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const groupLifecyclePolicy = {
  groupLifetimeInDays: 180,
  managedGroupTypes: "Selected",
  alternateNotificationEmails: "admin@contoso.com"
};

let res = await client.api('/groupLifecyclePolicies/{id}')
    .version('beta')
    .update({groupLifecyclePolicy : groupLifecyclePolicy});

```