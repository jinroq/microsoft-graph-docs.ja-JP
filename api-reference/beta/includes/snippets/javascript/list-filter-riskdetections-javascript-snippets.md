---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1112dce24b0f15761d91316acdd3bdc742bd40a7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725771"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/riskDetections')
    .version('beta')
    .filter('riskType eq 'unfamiliarFeatures' or riskLevel eq 'medium'')
    .get();

```