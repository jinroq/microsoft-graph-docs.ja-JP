---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 577f3781593969f17d8b41fdf11635e7fadd869c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475410"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartLineFormat = {
  color: "color-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/line')
    .version('beta')
    .update({workbookChartLineFormat : workbookChartLineFormat});

```