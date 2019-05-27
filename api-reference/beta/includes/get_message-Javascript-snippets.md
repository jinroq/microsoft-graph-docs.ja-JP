---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c57ae5d1231c2c9c6a867c6a286e91afe410b674
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448951"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkAGI1AAAoZCfHAAA=')
    .version('beta')
    .get();

```