---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4fb1fe8d34e02311ff2aa039a016d6a258d49891
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875041"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const publishedResource = {
    displayName: "New provisioning",
    resourceName: "domain1.contoso.com"
};

let res = await client.api('/onPremisesPublishingProfiles/provisioning/publishedResources')
    .version('beta')
    .post({publishedResource : publishedResource});

```