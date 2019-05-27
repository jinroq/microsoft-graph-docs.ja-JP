---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ed037660bde9478d01343fdd402ee85fa3743477
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34470106"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/children')
    .expand('thumbnails')
    .get();

```