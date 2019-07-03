---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bf34385fc458c019a243b672a38f66c47e1bae96
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471449"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChart = {
  type: "ColumnStacked",
  sourceData: "A1:B1",
  seriesBy: "Auto"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/add')
    .post(workbookChart);

```