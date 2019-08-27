---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 204e224e22cb1cac9aaec0cc65f1b3e3661b6c1a
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637793"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  parentReference: {
    id: "new-parent-folder-id"
  },
  name: "new-item-name.txt"
};

let res = await client.api('/me/drive/items/{item-id}')
    .version('beta')
    .update(driveItem);

```