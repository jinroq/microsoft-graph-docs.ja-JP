---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e0188059c57aa7cccca7ca0801ff86379fadadf5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730563"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const CommsOperation = {
  participants: [
    {
      endpointType: "default",
      identity: {
        user: {
          id: "550fae72-d251-43ec-868c-373732c2704f",
          tenantId: "72f988bf-86f1-41af-91ab-2d7cd011db47",
          displayName: "Heidi Steen"
        }
      },
      languageId: "languageId-value",
      region: "region-value",
      replacesCallId: "replacesCallId-value"
    }
  ],
  clientContext: "clientContext-value"
};

let res = await client.api('/app/calls/{id}/participants/invite')
    .version('beta')
    .post(CommsOperation);

```