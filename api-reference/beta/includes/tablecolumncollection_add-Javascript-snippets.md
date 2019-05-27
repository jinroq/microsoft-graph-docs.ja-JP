---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c23523306501f75247ccd0737240a69f699b0bf3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34482417"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableColumn = {
  index: {
  },
  values: [
    {
    }
  ]
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/add')
    .version('beta')
    .post(workbookTableColumn);

```