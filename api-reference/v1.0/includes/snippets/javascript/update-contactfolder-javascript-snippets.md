---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2c94e56bd1e6b21c7b21c9fea86064c49fded66f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740902"
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