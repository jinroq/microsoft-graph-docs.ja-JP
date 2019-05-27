---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 19a6ba5fb1a41f1b0a5fa37315caf50cdcc83e04
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469484"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  groupIds: [
    "groupIds-value"
  ]
};

let res = await client.api('/servicePrincipals/{id}/checkMemberGroups')
    .version('beta')
    .post(String);

```