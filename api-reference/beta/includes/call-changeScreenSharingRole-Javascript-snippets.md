---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6bc043e0c7999fa01e2368a0303b050ac79fa6e5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34456293"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const changeScreenSharingRole = {
  role: "viewer"
};

let res = await client.api('/app/calls/{id}/changeScreenSharingRole')
    .version('beta')
    .post(changeScreenSharingRole);

```