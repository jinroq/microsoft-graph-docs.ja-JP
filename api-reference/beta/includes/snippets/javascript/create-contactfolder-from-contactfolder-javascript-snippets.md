---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c82f8b7c73f8d346113249be4c79a56b8ac88777
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707398"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contactFolder = {
  displayName: "displayName-value"
};

let res = await client.api('/me/contactFolders/{id}/childFolders')
    .version('beta')
    .post({contactFolder : contactFolder});

```