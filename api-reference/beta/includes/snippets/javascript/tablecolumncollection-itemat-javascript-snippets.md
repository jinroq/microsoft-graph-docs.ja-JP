---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 29684bc0c2144c4eb1cf4f0e69cf6d31535854bf
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637887"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableColumn = {
  index: {
  }
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/ItemAt')
    .version('beta')
    .post(workbookTableColumn);

```