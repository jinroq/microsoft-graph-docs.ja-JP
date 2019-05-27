---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4b8bd1253ef6d793340ace080d0deb0329a3589e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461840"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeBorder = {
  color: "color-value",
  style: "style-value",
  sideIndex: "sideIndex-value",
  weight: "weight-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/borders/{sideIndex}')
    .version('beta')
    .update({workbookRangeBorder : workbookRangeBorder});

```