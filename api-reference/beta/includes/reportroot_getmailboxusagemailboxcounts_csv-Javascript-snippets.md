---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5e22b8dfec22959c7996e64356eae190434a7ea7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441998"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getMailboxUsageMailboxCounts(period='D7')')
    .version('beta')
    .get();

```