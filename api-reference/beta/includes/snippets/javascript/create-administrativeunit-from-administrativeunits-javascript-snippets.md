---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5e41d508a2a41d6e8e65957c54413b6dd7328eb5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710654"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const administrativeUnit = {
    displayName: "Seattle District Technical Schools",
    description: "Seattle district technical schools administration",
    visibility: "true"
};

let res = await client.api('/administrativeUnits')
    .version('beta')
    .post({administrativeUnit : administrativeUnit});

```