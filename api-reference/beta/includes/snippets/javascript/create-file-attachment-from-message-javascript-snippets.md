---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8e5fbe9bb42988962981337f9db73cdcf208267c
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/19/2019
ms.locfileid: "36462654"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  @odata.type: "#microsoft.graph.fileAttachment",
  name: "smile",
  contentBytes: "a0b1c76de9f7="
};

let res = await client.api('/me/messages/AAMkpsDRVK/attachments')
    .version('beta')
    .post({attachment : attachment});

```