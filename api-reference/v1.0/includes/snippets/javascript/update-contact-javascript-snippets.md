---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 16c1afc802e1b96ee7fa595fae16aa5f562b38d8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35495756"
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