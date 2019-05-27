---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a1dcb60b90ee4ecc91171e147c1a232b65ffdd1e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34477552"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names')
    .get();

```