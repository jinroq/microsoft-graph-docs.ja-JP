---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6b0e601dfc2637114e9352fb46dbbd4ff917fb0b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469379"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/sharedWithMe')
    .version('beta')
    .get();

```