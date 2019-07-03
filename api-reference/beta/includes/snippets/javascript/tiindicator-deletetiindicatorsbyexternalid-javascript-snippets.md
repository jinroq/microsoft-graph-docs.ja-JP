---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 897ab647ef64e7c745c2ba4fa0f9885905cac715
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485736"
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