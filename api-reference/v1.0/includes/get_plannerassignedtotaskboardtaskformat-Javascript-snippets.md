---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b5322c160e21ba425127504fe8cd1b4c9eec71a6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34451180"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/tasks/{task-id}/assignedToTaskBoardFormat')
    .get();

```