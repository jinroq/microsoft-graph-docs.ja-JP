---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bb0487d0d129ac4a0a378eb7d198b94a6fdea8f6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721594"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const messageRule = {
    displayName: "From partner",      
    sequence: 2,      
    isEnabled: true,          
    conditions: {
        senderContains: [
          "adele"       
        ]
     },
     actions: {
        forwardTo: [
          {
             emailAddress: {
                name: "Alex Wilbur",
                address: "AlexW@contoso.onmicrosoft.com"
              }
           }
        ],
        stopProcessingRules: true
     }    
};

let res = await client.api('/me/mailFolders/inbox/messagerules')
    .version('beta')
    .post({messageRule : messageRule});

```