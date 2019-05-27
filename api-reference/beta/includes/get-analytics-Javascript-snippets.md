---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6ed7779e22fbc5452d7d6b2adc0963855ecf232e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436461"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drives/{drive-id}/items/{item-id}/analytics')
    .version('beta')
    .get();

```