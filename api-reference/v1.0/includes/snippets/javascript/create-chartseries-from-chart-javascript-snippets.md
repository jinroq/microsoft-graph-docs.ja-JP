---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a00f32a51b19da622ae9d25d664c9e882ae19dc7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734110"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartSeries = {
  name: "name-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series')
    .post({workbookChartSeries : workbookChartSeries});

```