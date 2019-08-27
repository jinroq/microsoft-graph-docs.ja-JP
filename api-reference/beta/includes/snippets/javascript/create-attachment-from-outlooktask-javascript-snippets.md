---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 766070c2b1386bb1d1d9a32dc63cd77cde4d3293
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637928"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  lastModifiedDateTime: "datetime-value",
  name: "name-value",
  contentType: "contentType-value",
  size: 99,
  isInline: true
};

let res = await client.api('/users/{id}/outlook/tasks/{id}/attachments')
    .version('beta')
    .post(attachment);

```