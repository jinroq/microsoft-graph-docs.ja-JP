---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a1a2b65c182ae0ef09898e64518e3496e69c6e79
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442327"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getEmailAppUsageAppsUserCounts(period='D7')')
    .version('beta')
    .get();

```