---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c50139bfa4cbb99de947ffb241f7d7eb41d28c96
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731989"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reply = {
  comment: "comment-value"
};

let res = await client.api('/me/messages/{id}/reply')
    .post(reply);

```