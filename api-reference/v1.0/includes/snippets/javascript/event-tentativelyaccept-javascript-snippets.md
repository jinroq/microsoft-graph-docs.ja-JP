---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 250ed8115374fd6eb7589d0868bcfe8f2215b61a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735038"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tentativelyAccept = {
  comment: "comment-value",
  sendResponse: true
};

let res = await client.api('/me/events/{id}/tentativelyAccept')
    .post(tentativelyAccept);

```