---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d23a859c11cb3168e2434230b0d3f4d0ad002575
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724961"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators')
    .version('beta')
    .get();

```