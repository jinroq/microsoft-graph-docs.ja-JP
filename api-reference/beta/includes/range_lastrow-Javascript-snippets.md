---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: efa003c3b51660c0972c7edf16d5c25ea2247416
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442789"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/LastRow')
    .version('beta')
    .get();

```