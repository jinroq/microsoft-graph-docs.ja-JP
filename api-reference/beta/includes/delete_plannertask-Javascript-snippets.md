---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ada29f389bdb3d495a1ea961abea133f41a53274
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437623"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/tasks/'id'')
    .version('beta')
    .delete();

```