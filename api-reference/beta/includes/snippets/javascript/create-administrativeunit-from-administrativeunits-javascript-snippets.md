---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5e41d508a2a41d6e8e65957c54413b6dd7328eb5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35464596"
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