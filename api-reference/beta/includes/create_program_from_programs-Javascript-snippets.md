---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d6f979663b8d75efc0703740f3a92178cb64be1a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439835"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const program = {
    displayName: "testprogram3",
    description: "test description"
};

let res = await client.api('/programs')
    .version('beta')
    .post({program : program});

```