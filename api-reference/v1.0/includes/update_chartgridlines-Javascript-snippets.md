---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0b330af128f75affed54d37a40e8b47b1e7de6ec
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34467269"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartGridlines = {
  visible: true
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/minorGridlines')
    .update({workbookChartGridlines : workbookChartGridlines});

```