---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 897ab647ef64e7c745c2ba4fa0f9885905cac715
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34468775"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const ResultInfo = {
  value: [
    "externalId-value1",
    "externalId-value2"
  ]
};

let res = await client.api('/security/tiIndicators/deleteTiIndicatorsByExternalId')
    .version('beta')
    .post(ResultInfo);

```