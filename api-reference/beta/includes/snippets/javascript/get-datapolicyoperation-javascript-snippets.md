---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0c282631f50e5ac46a84298651a0f5ba6b64c9e0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707048"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/dataPolicyOperations/{id}')
    .version('beta')
    .get();

```