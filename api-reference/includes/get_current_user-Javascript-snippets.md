---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fdcaa49e6ac75c2c1e9bb4060ea7a28208a92ce1
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34843550"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me')
    .get();

```