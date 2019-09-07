---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 081bf8acfc769792bb227fd8465c6f6796883bbd
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/07/2019
ms.locfileid: "36791146"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const call = {
  callbackUri: "https://bot.contoso.com/api/calls",
  mediaConfig: {
    @odata.type: "#microsoft.graph.serviceHostedMediaConfig"
  },
  targets: [
    {
      @odata.type: "#microsoft.graph.participantInfo",
      identity: {
        @odata.type: "#microsoft.graph.identitySet",
        user: {
          @odata.type: "#microsoft.graph.identity",
          displayName: "John",
          id: "112f7296-5fa4-42ca-bae8-6a692b15d4b8"
        }
      }
    }
  ],
  requestedModalities: [
    "audio"
  ]
};

let res = await client.api('/app/calls')
    .version('beta')
    .post(call);

```