---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f85aec8668b3e2a961e29cf3ca4ebebfe7b49e3e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739626"
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