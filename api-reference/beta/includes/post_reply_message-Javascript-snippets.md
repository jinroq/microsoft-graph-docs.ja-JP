---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 31d04c8ebca9b1f709bc93a8092ff32e509ae937
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443279"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chatMessage = {
  body: {
    contentType: "html",
    content: "Hello World"
  }
};

let res = await client.api('/teams/{id}/channels/{id}/messages/{id}/replies')
    .version('beta')
    .post({chatMessage : chatMessage});

```