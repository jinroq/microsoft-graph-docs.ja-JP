---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 083f6c8c50c88aa2c1000d5c23613601a6c7c08e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34476215"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  recipients: [
    {
      email: "ryan@contoso.com"
    }
  ],
  message: "Here's the file that we're collaborating on.",
  requireSignIn: true,
  sendInvitation: true,
  roles: [ "write" ]
};

let res = await client.api('/me/drive/items/{item-id}/invite')
    .post(permission);

```