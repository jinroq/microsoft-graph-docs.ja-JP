---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 49ab3517373d3ba314d6f7582e463693413688ad
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34482389"
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
    .post({workbookTableColumn : workbookTableColumn});

```