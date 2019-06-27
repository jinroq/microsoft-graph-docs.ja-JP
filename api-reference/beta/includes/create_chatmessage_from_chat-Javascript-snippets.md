---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 852e03ce852f463551575f8de14e7a90203676c1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35320028"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chatMessage = {
  body: {
     "content" : "Hello world"
  }
};

let res = await client.api('/teams/{id}/channels/{id}/messages')
    .version('beta')
    .post({chatMessage : chatMessage});

```