---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 24c6c955b34fab32ac3e9c118bd858d15eb347ea
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465959"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/start')
    .version('beta')
    .post();

```