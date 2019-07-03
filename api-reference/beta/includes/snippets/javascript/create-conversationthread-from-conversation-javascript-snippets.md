---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 15fc8f8a746d4fbeafc853f76d46d74a3e45a06d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486675"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationThread = {
  topic: "topic-value",
  posts: [{
      body: {
        contentType: "html",
        content: "this is body content"
      }
  }]
};

let res = await client.api('/groups/{id}/conversations/{id}/threads')
    .version('beta')
    .post({conversationThread : conversationThread});

```