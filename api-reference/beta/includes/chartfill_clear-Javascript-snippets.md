---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 56834e164694d525d8d590b709921d9c5811fd75
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474780"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/clear')
    .version('beta')
    .post();

```