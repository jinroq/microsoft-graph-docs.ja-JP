---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3553749da5dcc97c16fa750569b2221a81773d1a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447776"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/buckets/hsOf2dhOJkqyYYZEtdzDe2QAIUCR')
    .version('beta')
    .get();

```