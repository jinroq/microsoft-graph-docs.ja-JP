---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d1eda9876a7a526af495478e6baf5669389e299d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444819"
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

let res = await client.api('/groups/{id}/checkMemberGroups')
    .version('beta')
    .post(String);

```