---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e83537ac61707828bdbe183a364c0fcd789a6a8e
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637747"
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
    .update(identityProvider);

```