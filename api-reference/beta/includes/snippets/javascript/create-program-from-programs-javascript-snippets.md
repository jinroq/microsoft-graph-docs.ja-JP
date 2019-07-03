---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d6f979663b8d75efc0703740f3a92178cb64be1a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35503577"
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