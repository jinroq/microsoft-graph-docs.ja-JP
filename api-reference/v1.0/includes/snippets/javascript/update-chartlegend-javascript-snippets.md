---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 76bc12afb8fcf7fbe9e06c3b395da9c9752ebdd9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35495765"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartLegend = {
  visible: true,
  position: "position-value",
  overlay: true
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend')
    .update({workbookChartLegend : workbookChartLegend});

```