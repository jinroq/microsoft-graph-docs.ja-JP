---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9a1c3f91b02f29738172efee1200c685bff84743
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709028"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const CommsOperation = {
  all: true,
  clientContext: "clientContext-value"
};

let res = await client.api('/app/calls/{id}/cancelMediaProcessing')
    .version('beta')
    .post(CommsOperation);

```