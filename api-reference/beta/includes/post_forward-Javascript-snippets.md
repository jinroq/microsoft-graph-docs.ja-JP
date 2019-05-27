---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9ee25866fdaa118aa06bfc120770205fceeaaf94
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443461"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const forward = {
  comment: "comment-value",
  toRecipients: [
    {
      emailAddress: {
        name: "name-value",
        address: "address-value"
      }
    }
  ]
};

let res = await client.api('/groups/{id}/threads/{id}/posts/{id}/forward')
    .version('beta')
    .post(forward);

```