---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e405405786ff922db56683bfdc117365cde0a7be
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461356"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  parentReference: {
    id: "{new-parent-folder-id}"
  },
  name: "new-item-name.txt"
};

let res = await client.api('/me/drive/items/{item-id}')
    .update({driveItem : driveItem});

```