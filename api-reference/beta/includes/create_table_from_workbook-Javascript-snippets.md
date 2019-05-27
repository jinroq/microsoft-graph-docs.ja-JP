---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e7dc9a684cfa43f11008f6151ac0e9c773904e94
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439394"
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