---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a7317f50118bf5ea405ae0b19c289dd342f4c626
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637778"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
    @odata.type: "#microsoft.graph.referenceAttachment",
    name: "Personal pictures",
    sourceUrl: "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
    providerType: "oneDriveConsumer",
    permission: "Edit",
    isFolder: "True"
};

let res = await client.api('/me/events/AAMkAGE1M88AADUv0uAAAG=/attachments')
    .version('beta')
    .post(attachment);

```