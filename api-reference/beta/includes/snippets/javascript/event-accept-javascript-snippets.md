---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8c6ae08e66e0420b5226a83f6224513e118c3aed
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714350"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accept = {
  comment: "comment-value",
  sendResponse: true
};

let res = await client.api('/me/events/{id}/accept')
    .version('beta')
    .post(accept);

```