---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9e159ec1f494217cd0b843031c4bd4254f62a547
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475144"
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
    .update({workbookTable : workbookTable});

```