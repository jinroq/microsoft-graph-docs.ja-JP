---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b3f9728e237800e3ea2617952e3e7c469765ad76
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442985"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const clear = {
  applyTo: "applyTo-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/clear')
    .version('beta')
    .post(clear);

```