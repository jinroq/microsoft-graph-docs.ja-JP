---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c50139bfa4cbb99de947ffb241f7d7eb41d28c96
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461476"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reply = {
  comment: "comment-value"
};

let res = await client.api('/me/messages/{id}/reply')
    .post(reply);

```