---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 19477d8fab0d4c3095f97385817264ff7e491351
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861351"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  type: "view",
  password: "ThisIsMyPrivatePassword",
  scope: "anonymous"
};

let res = await client.api('/me/drive/items/{itemId}/createLink')
    .version('beta')
    .post(permission);

```