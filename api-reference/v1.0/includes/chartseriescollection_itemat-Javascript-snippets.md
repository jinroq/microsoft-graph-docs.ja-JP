---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a79f8178f55b1c417e9ecd59ca52163f95671f54
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34467073"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartSeries = {
  index: 2
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/itemAt')
    .post({workbookChartSeries : workbookChartSeries});

```