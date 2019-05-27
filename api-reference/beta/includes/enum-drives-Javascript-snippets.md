---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8d85bd1d682dd5c28465c4814141fa97692905cb
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436853"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drives')
    .version('beta')
    .get();

```