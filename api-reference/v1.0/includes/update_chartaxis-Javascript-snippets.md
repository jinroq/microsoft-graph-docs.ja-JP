---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f18f528747d77c9a4485aae87560d2d3c69efe7a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449686"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartAxis = {
  majorUnit: {
  },
  maximum: {
  },
  minimum: {
  }
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis')
    .update({workbookChartAxis : workbookChartAxis});

```