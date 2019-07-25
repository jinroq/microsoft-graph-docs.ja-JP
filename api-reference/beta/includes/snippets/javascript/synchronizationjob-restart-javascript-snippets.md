---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 663ba91ace2e3de1f18d508291a98e6764d83308
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869280"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const restart = {
   criteria: {
       resetScope: "Watermark, Escrows, QuarantineState"
   }
};

let res = await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/restart')
    .version('beta')
    .post(restart);

```