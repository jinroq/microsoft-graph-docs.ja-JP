---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 809173ab178f0fcd0697117fa989339300954f0d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442390"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getEmailActivityUserCounts(period='D7')')
    .version('beta')
    .get();

```