---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 82fc62d301155f5fe1b31b3ecf2e1b899dfbea0d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448168"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contacts/{id}')
    .version('beta')
    .get();

```