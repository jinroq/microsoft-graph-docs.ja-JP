---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 472b6d69d00c685e621295cb0ff43a6b05372779
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723896"
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

let res = await client.api('/me/contactFolders')
    .version('beta')
    .post({contactFolder : contactFolder});

```