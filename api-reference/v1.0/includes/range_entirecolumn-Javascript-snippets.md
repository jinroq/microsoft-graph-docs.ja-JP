---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 663077ea71383a76e28c0ad8c14baa253b408282
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34450933"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/entireColumn')
    .get();

```