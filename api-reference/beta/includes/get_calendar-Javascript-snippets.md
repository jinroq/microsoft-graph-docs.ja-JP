---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3b2893395be79e6c0c4c7af22e2782f37b8524bb
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34473569"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendar')
    .version('beta')
    .get();

```