---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7b487772ccbd2aeb63ca97d5b64fdec95503d1c7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715594"
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
    .post({conversationThread : conversationThread});

```