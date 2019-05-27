---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0e8fa04fa0375084b2dab3155e468b0bad7591e0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457095"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contact = {
  givenName: "Pavel",
  surname: "Bansky",
  emailAddresses: [
    {
      address: "pavelb@contoso.onmicrosoft.com",
      name: "Pavel Bansky",
      type: "personal"
    },
    {
      address: "pavelb@fabrikam.onmicrosoft.com",
      name: "Pavel Bansky",
      type: "other",
      otherLabel: "Volunteer work"
    }
  ],
  "phones" : [
    {
      number: "+1 732 555 0102",
      type: "business"
    }
  ]
};

let res = await client.api('/me/contacts')
    .version('beta')
    .post({contact : contact});

```