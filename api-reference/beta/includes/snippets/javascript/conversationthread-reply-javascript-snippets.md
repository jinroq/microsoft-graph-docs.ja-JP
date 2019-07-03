---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: caadfe9c2a63e8cd8e4899b0571f152769d9abed
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35464605"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reply = {
  post: {
    body: {
      contentType: "",
      content: "content-value"
    }
  }
};

let res = await client.api('/groups/{id}/threads/{id}/reply')
    .version('beta')
    .post(reply);

```