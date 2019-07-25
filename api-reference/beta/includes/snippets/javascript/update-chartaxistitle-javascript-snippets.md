---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 43a19a16257bfeedbefb0fcc44bf17b8069f1769
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708316"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartAxisTitle = {
  text: "text-value",
  visible: true
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/title')
    .version('beta')
    .update({workbookChartAxisTitle : workbookChartAxisTitle});

```