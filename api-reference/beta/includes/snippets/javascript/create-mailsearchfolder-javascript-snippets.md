---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 08684cbe8a908af22c8197762d7075b3e5cba249
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637988"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  @odata.type: "microsoft.graph.mailSearchFolder",
  displayName: "Weekly digests",
  includeNestedFolders: true,
  sourceFolderIds: ["AQMkADYAAAIBDAAAAA=="],
  filterQuery: "contains(subject, 'weekly digest')"
};

let res = await client.api('/me/mailfolders/AQMkADYAAAIBDAAAAA==/childfolders')
    .version('beta')
    .post(mailFolder);

```