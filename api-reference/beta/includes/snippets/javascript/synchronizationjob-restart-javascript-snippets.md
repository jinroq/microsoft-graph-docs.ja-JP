---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 42abf7b86246e6b8a1471cd55e2f7100380f676a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485562"
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