---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 712eb021795feda8f76d5ec6385f4532a67e34e4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460223"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeBorder = {
  id: "id-value",
  color: "color-value",
  style: "style-value",
  sideIndex: "sideIndex-value",
  weight: "weight-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/borders')
    .post({workbookRangeBorder : workbookRangeBorder});

```