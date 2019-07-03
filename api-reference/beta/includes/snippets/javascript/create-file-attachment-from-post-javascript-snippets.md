---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 44fd630a038f92cd8ec25c6acbd59a5051b52f92
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485651"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  @odata.type: "#microsoft.graph.fileAttachment",
  name: "name-value",
  contentBytes: "contentBytes-value"
};

let res = await client.api('/groups/{id}/threads/{id}/posts/{id}/attachments')
    .version('beta')
    .post({attachment : attachment});

```