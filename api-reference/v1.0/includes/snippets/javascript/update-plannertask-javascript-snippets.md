---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bea4714cc1f9f50cc0d576555977857324898947
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471542"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerTask = {
  assignments: {
    fbab97d0-4932-4511-b675-204639209557: {
      @odata.type: "#microsoft.graph.plannerAssignment",
      orderHint: "N9917 U2883!"
    }
  },
  appliedCategories: {
    category3: true,
    category4: false
  }
};

let res = await client.api('/planner/tasks/{task-id}')
    .update({plannerTask : plannerTask});

```