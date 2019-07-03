---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d0ec590af3d1ebbb4a765565199942d7725b0c93
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486674"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationThread = {
  topic: "New Conversation Thread Topic",
  posts: [{
    body: {
      contentType: "html",
      content: "this is body content"
    },
    newParticipants: [{
      emailAddress: {
        name: "Alex Darrow",
        address: "alexd@contoso.com"
      }
    }]
  }]
};

let res = await client.api('/groups/{id}/threads')
    .version('beta')
    .post({conversationThread : conversationThread});

```