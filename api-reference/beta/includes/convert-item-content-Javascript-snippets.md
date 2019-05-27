---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 21a808483142572ec816f9838ed21b79bea027fe
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460883"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/items/{item-id}/content')
    .version('beta')
    .get();

```