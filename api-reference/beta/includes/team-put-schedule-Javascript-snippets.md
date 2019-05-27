---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 380160445735d725747814b74cf68668ebc5e43e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469301"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const schedule = {
  enabled: true,
  timeZone: "America/Chicago"
};

let res = await client.api('/teams/{teamId}/schedule')
    .version('beta')
    .put({schedule : schedule});

```