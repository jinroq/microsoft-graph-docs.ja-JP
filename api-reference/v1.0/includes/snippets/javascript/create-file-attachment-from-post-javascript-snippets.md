---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f85aec8668b3e2a961e29cf3ca4ebebfe7b49e3e
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36634157"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  @odata.type: "#microsoft.graph.fileAttachment",
  name: "name-value",
  contentBytes: "base64-contentBytes-value"
};

let res = await client.api('/groups/{id}/threads/{id}/posts/{id}/attachments')
    .post({attachment : attachment});

```