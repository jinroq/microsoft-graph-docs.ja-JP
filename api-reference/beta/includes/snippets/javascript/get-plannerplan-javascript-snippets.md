---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 28d1a7d5e212209c25b316c7ac0f353d1ee06ffa
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730387"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/plans/'id'')
    .version('beta')
    .get();

```