---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 12e937d4931a8f7217bec201dbc5e6a087d85653
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713498"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id:"https://graph.microsoft.com/beta/users/alexd@contoso.com"
};

let res = await client.api('/groups/{id}/rejectedSenders/$ref')
    .version('beta')
    .post({directoryObject : directoryObject});

```