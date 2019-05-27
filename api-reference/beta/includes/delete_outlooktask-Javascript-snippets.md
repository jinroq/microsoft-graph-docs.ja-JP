---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fb24eaac349928e1e0f6570681c65344ba6ee3c0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437868"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/tasks/AAMkADIyAAAhrb_QAAA=')
    .version('beta')
    .delete();

```