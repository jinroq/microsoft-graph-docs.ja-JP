---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 76bc12afb8fcf7fbe9e06c3b395da9c9752ebdd9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735449"
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