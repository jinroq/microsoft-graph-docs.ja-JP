---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 268b8c52bab21f2f238d0d4ceb8c3af54d996e58
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34451974"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const CommsOperation = {
  clientContext: "clientContext-value"
};

let res = await client.api('/app/calls/{id}/unmute')
    .version('beta')
    .post(CommsOperation);

```