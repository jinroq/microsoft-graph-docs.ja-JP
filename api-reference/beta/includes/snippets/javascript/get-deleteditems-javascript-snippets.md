---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: aed27b815116d4f792bc4f7b7e46f9fec7c729be
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706916"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directory/deleteditems/microsoft.graph.group')
    .version('beta')
    .get();

```