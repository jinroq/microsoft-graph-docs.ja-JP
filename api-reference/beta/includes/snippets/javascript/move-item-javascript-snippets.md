---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6cfa6c5e1b51d8b280036455a958f2e4025e1034
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486765"
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
    .update({driveItem : driveItem});

```