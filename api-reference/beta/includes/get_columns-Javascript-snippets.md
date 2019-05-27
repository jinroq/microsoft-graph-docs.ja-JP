---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c5146959d51be22b369ae0ec68b786834f44712e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472617"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns')
    .version('beta')
    .skip(5)
    .top(5)
    .get();

```