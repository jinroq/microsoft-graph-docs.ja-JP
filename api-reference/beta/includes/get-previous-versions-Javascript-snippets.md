---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: db6b92ff1baf16be8989c526fb75b4652dd67cfc
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474703"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/versions')
    .version('beta')
    .get();

```