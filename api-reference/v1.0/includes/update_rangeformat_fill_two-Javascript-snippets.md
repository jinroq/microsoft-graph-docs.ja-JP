---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 760cdc66fcd57338feaca3d8ca1511225645c721
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34468178"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFill = {
  color: "#00FF00"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$B$1')/format/fill')
    .update({workbookRangeFill : workbookRangeFill});

```