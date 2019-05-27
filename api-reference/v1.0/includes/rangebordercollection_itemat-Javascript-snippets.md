---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: eddf334e15c58a42f961d03f4a7f94443ed13db3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469654"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeBorder = {
  index: 1
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/borders/itemAt')
    .post({workbookRangeBorder : workbookRangeBorder});

```