---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fb25f1360fe346df752e93ab70375326fcc7c83d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449254"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/joinedTeams')
    .version('beta')
    .get();

```