---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 16c1afc802e1b96ee7fa595fae16aa5f562b38d8
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741028"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contact = {
  homeAddress: {
    street: "123 Some street",
    city: "Seattle",
    state: "WA",
    postalCode: "98121"
  },
  birthday: "1974-07-22"
};

let res = await client.api('/me/contacts/{id}')
    .update({contact : contact});

```