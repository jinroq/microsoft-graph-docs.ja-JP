---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: af518bf1ab80fdf6ee3a6bf86b3b96fa88d5dd6d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732131"
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

let res = await client.api('/me/messages/{id}/forward')
    .post(forward);

```