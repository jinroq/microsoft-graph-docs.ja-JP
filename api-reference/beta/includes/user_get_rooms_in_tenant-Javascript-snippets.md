---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ab52f9899b1df42a3adeb2c72b17f844b2b0fbfb
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480282"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/findRooms')
    .version('beta')
    .get();

```