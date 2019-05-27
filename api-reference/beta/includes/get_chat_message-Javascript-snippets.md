---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3fac72fb98be0a82a0e2480ad3efd5d76ba79c5e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472820"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/chats/{id}')
    .version('beta')
    .get();

```