---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e04bef844e279ab8a0123ca6e064b35ddee1a3a0
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461973"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  @odata.type: "#microsoft.graph.fileAttachment",
  name: "smile",
  contentBytes: "R0lGODdhEAYEAA7"
};

let res = await client.api('/me/messages/AAMkpsDRVK/attachments')
    .post({attachment : attachment});

```