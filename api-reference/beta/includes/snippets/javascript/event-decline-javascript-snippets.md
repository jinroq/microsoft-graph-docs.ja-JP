---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0582e0d132931805a3ce3a5e0e0c9e65267f1fe2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714370"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const decline = {
  comment: "comment-value",
  sendResponse: true
};

let res = await client.api('/me/events/{id}/decline')
    .version('beta')
    .post(decline);

```