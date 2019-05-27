---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2988460caff6334ebf137ee903665eee3b34d5e1
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34483262"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{siteId}/drive')
    .version('beta')
    .get();

```