---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c6c2aa567c85d1b48c343b0b8c7953dd9ce7ec69
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463772"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getTeamsDeviceUsageUserCounts(period='D7')')
    .version('beta')
    .get();

```