---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3ab3af58ea169327e4c8f8cab40419dd11e9e124
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705139"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerAssignedToTaskBoardTaskFormat = {
  orderHintsByAssignee: {
    aaa27244-1db4-476a-a5cb-004607466324: "8566473P 957764Jk!"
  }
};

let res = await client.api('/planner/tasks/{task-id}/assignedToTaskBoardFormat')
    .update({plannerAssignedToTaskBoardTaskFormat : plannerAssignedToTaskBoardTaskFormat});

```