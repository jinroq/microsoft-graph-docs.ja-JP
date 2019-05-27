---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3fb8aa55d6ea5af1347404dff8f1fef8312cb98d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447384"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoleAssignments/{id}')
    .version('beta')
    .get();

```