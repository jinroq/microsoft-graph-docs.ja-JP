---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 20f23ea894937ea1c9b9d93b0d314402d84a1d53
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724751"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTable = {
  name: "name-value",
  showHeaders: true,
  showTotals: true,
  style: "style-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}')
    .version('beta')
    .update({workbookTable : workbookTable});

```