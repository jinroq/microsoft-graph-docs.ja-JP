---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: eeb8cd0e3a19e639811352a45f9b44e4a6b59bb9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739668"
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
    .post(forward);

```