---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3c97be728ff7b6f21ffd948334b64db8aa966bf0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446198"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}')
    .version('beta')
    .get();

```