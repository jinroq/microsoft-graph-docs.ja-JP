---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e7dc9a684cfa43f11008f6151ac0e9c773904e94
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723805"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTable = {
  address: "A1:D8",
  hasHeaders: false
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/$/add')
    .version('beta')
    .post(workbookTable);

```