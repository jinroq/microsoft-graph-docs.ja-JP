---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e09613a2363b5af1a2c13b71254121b04b7c2565
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705319"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProvider = {
    clientSecret: "1111111111111"
};

let res = await client.api('/identityProviders/Amazon-OAuth')
    .version('beta')
    .update({identityProvider : identityProvider});

```