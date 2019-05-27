---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d63ba97ad9376231971f3dae76fa1dc57b984cf3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34476418"
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

let res = await client.api('/me/checkMemberGroups')
    .version('beta')
    .post(String);

```