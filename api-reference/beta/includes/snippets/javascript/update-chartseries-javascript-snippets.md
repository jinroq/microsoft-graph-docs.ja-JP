---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0736d8d4606c6c5cf7d40c1a5966e03af8a70abe
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707866"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartSeries = {
  name: "name-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}')
    .version('beta')
    .update({workbookChartSeries : workbookChartSeries});

```