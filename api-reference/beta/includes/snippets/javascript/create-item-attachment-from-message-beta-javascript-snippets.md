---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d8a0f6c4516bd96119f2d0bf2e602599e1de69c2
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633504"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  @odata.type: "#microsoft.graph.itemAttachment",
  name: "Holiday event", 
  item: {
    @odata.type: "microsoft.graph.event",
    subject: "Discuss gifts for children",
    body: {
      contentType: "HTML",
      content: "Let's look for funding!"
    },
    start: {
      dateTime: "2016-12-02T18:00:00",
      timeZone: "Pacific Standard Time"
    },
    end: {
      dateTime: "2016-12-02T19:00:00",
      timeZone: "Pacific Standard Time"
    }
  }
};

let res = await client.api('/me/messages/AAMkpsDRVK/attachments')
    .version('beta')
    .post(attachment);

```