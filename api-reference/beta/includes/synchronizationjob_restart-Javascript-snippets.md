---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 42abf7b86246e6b8a1471cd55e2f7100380f676a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465966"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const restart = {
   criteria: {
       resetScope: "ConnectorDataStore, Escrows, QuarantineState"
   }
};

let res = await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/restart')
    .version('beta')
    .post(restart);

```