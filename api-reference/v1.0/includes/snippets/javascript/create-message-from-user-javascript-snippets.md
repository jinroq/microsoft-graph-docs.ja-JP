---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 77e9a3a47ea4ec5bc693726ebfa7c453688900a4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471362"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
    subject:"Did you see last night's game?",
    importance:"Low",
    body:{
        contentType:"HTML",
        content:"They were <b>awesome</b>!"
    },
    toRecipients:[
        {
            emailAddress:{
                address:"AdeleV@contoso.onmicrosoft.com"
            }
        }
    ]
};

let res = await client.api('/me/messages')
    .post({message : message});

```