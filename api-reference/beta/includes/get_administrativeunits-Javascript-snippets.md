---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0a273d9e16fbfecd2c73997ced3c505684539a91
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474248"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/administrativeUnits')
    .version('beta')
    .get();

```