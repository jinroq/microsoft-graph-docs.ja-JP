---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 47a39811a3f65ef701777351aad0871ebd74c228
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718318"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/riskyUsers/c2b6c2b9-dddc-acd0-2b39-d519d803dbc3')
    .version('beta')
    .get();

```