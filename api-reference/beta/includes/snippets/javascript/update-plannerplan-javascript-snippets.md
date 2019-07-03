---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bddebd3ebb8600ca259c102281a063e74d5658ab
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35503501"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerPlan = {
  title: "title-value"
};

let res = await client.api('/planner/plans/'id'')
    .version('beta')
    .update({plannerPlan : plannerPlan});

```