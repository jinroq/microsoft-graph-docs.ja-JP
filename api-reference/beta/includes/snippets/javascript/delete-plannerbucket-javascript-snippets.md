---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0976ea0975fecee37c47a17e14d7f77daf7fc6a3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730430"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/buckets/'id'')
    .version('beta')
    .delete();

```