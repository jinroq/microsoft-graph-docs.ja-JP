---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d35797e52c3b516d0318a9206b22361f4e1cf95a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732379"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  displayName: "displayName-value",
};

let res = await client.api('/me/mailFolders/{id}/childFolders')
    .post({mailFolder : mailFolder});

```