---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0772aa2e4c1b7f218654082f6aec1c3cd35e39a8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445533"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/sort')
    .version('beta')
    .get();

```