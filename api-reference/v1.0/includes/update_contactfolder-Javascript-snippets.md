---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2c94e56bd1e6b21c7b21c9fea86064c49fded66f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475757"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contactFolder = {
  parentFolderId: "parentFolderId-value",
  displayName: "displayName-value"
};

let res = await client.api('/me/contactFolders/{id}')
    .update({contactFolder : contactFolder});

```