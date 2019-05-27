---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 416f6681bff3d5bed67716dff41c77b3154a15cf
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34476159"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartDataLabels = {
  position: "position-value",
  showValue: true,
  showSeriesName: true,
  showCategoryName: true,
  showLegendKey: true
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/datalabels')
    .version('beta')
    .update({workbookChartDataLabels : workbookChartDataLabels});

```