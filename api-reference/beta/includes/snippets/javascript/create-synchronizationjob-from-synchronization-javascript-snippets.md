---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: eb125b9b027cdb5d3f27765065301830317cb82e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717346"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const synchronizationJob = {
    templateId: "BoxOutDelta"
};

let res = await client.api('/servicePrincipals/{id}/synchronization/jobs')
    .version('beta')
    .post({synchronizationJob : synchronizationJob});

```