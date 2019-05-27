---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ecc360f08bc57f2417da3b3191f2f8312d89a74b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448357"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/oAuth2Permissiongrants')
    .version('beta')
    .get();

```