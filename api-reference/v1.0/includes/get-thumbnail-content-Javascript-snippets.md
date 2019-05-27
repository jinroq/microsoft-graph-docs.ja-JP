---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 21363560b6efd0e3e9909158cc012ee433ac9410
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34470156"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content')
    .get();

```