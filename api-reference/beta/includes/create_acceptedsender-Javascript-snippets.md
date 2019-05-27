---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: dc7d8c88121ee95591ea1988708d350fadb0ec34
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475529"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id:"https://graph.microsoft.com/beta/users/alexd@contoso.com"
};

let res = await client.api('/groups/{id}/acceptedSenders/$ref')
    .version('beta')
    .post({directoryObject : directoryObject});

```