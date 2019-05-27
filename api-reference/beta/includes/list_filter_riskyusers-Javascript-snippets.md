---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 64df205982730e669bb75ab9f5ec5cad389477fe
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444308"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/riskyUsers')
    .version('beta')
    .filter('riskLevel eq microsoft.graph.riskLevel'medium'')
    .get();

```