---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 25072828b01ee4669bc02c3d2b39bc6f32e86b37
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737289"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartFont = {
  bold: true,
  color: "color-value",
  italic: true,
  name: "name-value",
  size: 99,
  underline: "underline-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/format/font')
    .update({workbookChartFont : workbookChartFont});

```