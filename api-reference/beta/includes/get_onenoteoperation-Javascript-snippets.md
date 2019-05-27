---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 66255c8734ce710555129cfb5b3a8253c4c7d41d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448308"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/operations/{id}')
    .version('beta')
    .get();

```