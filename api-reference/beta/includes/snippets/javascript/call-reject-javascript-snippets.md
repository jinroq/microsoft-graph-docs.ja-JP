---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 214c0a91ee4ab17c0f480c2c40992e6b2602554e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708832"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reject = {
  reason: "none"
};

let res = await client.api('/app/calls/{id}/reject')
    .version('beta')
    .post(reject);

```