---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 508db2f1f43b92aaf1c7d4d9eb07ea978a2cdfa1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35464589"
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
    .version('beta')
    .post({mailFolder : mailFolder});

```