---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a1bd8b70883aefeae797752f6c2b31e0f37e8d22
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443090"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoleAssignmentRequests/my')
    .version('beta')
    .get();

```