---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 821bbde6faef4ed73d03b91bb2cc3b179551faee
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637817"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartPoint = {
  index: {
  }
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points/ItemAt')
    .version('beta')
    .post(workbookChartPoint);

```