---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f69cfc9636fe5e6c977b293576501aacf7f2ee07
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724520"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const ResultInfo = {
  value: [
    "id-value1",
    "id-value2"
  ]
};

let res = await client.api('/security/tiIndicators/deleteTiIndicators')
    .version('beta')
    .post(ResultInfo);

```