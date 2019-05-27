---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ee2ff962a98f4a4d0cdf3b2429d9131a8da22787
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34451124"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/photos')
    .get();

```