---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: de7731ee3547cc129c068a494e36972ba82eb402
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441907"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getMailboxUsageQuotaStatusMailboxCounts(period='D7')')
    .version('beta')
    .get();

```