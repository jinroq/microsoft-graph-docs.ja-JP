---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a568d6229153de65eac71e9288a5e585568e4b3a
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637826"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChart = {
  height: 99,
  left: 99
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}')
    .version('beta')
    .update(workbookChart);

```