---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4cd78eed61ab4c12c61c2403bc811f854550a1e2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472568"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contacts/AAMkAGI2THk0AAA=')
    .version('beta')
    .get();

```