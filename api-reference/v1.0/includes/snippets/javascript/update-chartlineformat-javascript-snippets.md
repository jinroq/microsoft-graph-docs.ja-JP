---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cfb0d39e4deb7b97c75d703ab70fe71ef1cc6c36
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735384"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartLineFormat = {
  color: "color-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesAxis/format/line')
    .update({workbookChartLineFormat : workbookChartLineFormat});

```