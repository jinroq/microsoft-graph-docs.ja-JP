---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6b7e32087895b59336fb3894d3c9ce250037b856
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34458344"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/schemaExtensions/{id}')
    .delete();

```