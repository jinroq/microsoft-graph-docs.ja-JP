---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cedf0d8ef9638eb065d7ba720949f14c943ebeed
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34478805"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')')
    .version('beta')
    .get();

```