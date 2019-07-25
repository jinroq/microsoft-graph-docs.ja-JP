---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2fb35c5a2aeaea10dc577207687443ed1cdafbe5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885511"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id:"https://graph.microsoft.com/v1.0/users/alexd@contoso.com"
};

let res = await client.api('/groups/{id}/rejectedSenders/$ref')
    .post({directoryObject : directoryObject});

```