---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 771ab96dbfa19856e1d8f5a9596c19873c47b576
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734749"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/tasks/{task-id}/details')
    .get();

```