---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2a0c43c22946468494f94db70e041f5894ca3423
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734419"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerBucket = {
  name: "Development"
};

let res = await client.api('/planner/buckets/{bucket-id}')
    .update({plannerBucket : plannerBucket});

```