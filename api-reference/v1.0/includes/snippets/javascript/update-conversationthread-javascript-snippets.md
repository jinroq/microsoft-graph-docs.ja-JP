---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 35b88d21c7f7f6fc59e72e629de0c670ab46c130
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733697"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationThread = {
  @odata.type:"#Microsoft.OutlookServices.ConversationThread",
  isLocked: true
};

let res = await client.api('/groups/{id}/threads/{id}')
    .update({conversationThread : conversationThread});

```