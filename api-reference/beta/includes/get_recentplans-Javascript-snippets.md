---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 18163aa07fa813d89e642b7a68b10b4c56fe46d0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446929"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/planner/recentPlans')
    .version('beta')
    .get();

```