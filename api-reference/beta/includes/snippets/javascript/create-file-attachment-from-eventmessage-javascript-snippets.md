---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7d19472b6cf551e8074325df68fecb8b7ecd280f
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637772"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  @odata.type: "#Microsoft.OutlookServices.FileAttachment",
  name: "name-value",
  contentType: "contentType-value",
  isInline: false,
  contentLocation: "contentLocation-value",
  contentBytes: "contentBytes-value"
};

let res = await client.api('/me/messages/{id}/attachments')
    .version('beta')
    .post(attachment);

```