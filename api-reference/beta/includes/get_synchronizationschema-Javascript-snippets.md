---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4d537c365d2e65bd6d1301f6656d85775429eda0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445757"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema')
    .version('beta')
    .header('Authorization','Bearer {Token}')
    .get();

```