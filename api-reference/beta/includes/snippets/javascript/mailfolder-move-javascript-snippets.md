---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2efcbf125863b0e5120bf22048cfd8a7d2b327ee
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721636"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  destinationId: "destinationId-value"
};

let res = await client.api('/me/mailFolders/{id}/move')
    .version('beta')
    .post(mailFolder);

```