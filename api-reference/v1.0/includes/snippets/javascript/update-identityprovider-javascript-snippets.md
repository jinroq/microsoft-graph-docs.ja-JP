---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 92d7223a8e52cf33bcdebb99421aceca0ab385cf
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731590"
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
    .update({identityProvider : identityProvider});

```