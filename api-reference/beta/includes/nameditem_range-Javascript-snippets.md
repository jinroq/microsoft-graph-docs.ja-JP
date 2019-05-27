---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b3308613031b767470cfccac5dc560c731a0c308
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443825"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/Range')
    .version('beta')
    .post();

```