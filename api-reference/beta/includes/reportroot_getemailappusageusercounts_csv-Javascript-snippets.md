---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 00c1580c9d377bc2ceef004f8e4dfea47bce94f3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442208"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getEmailAppUsageUserCounts(period='D7')')
    .version('beta')
    .get();

```