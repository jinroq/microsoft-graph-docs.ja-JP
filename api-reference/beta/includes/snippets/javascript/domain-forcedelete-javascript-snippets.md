---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cbffeceb7f1572ccc91517881096a3e39f7e4106
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706402"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const forceDelete = {
  disableUserAccounts: true
};

let res = await client.api('/domains/contoso.com/forceDelete')
    .version('beta')
    .post(forceDelete);

```