---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a79f8178f55b1c417e9ecd59ca52163f95671f54
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471214"
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