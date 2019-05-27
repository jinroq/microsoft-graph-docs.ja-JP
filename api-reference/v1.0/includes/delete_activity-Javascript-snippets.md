---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 88109a17c9a88224081e8023cb2796e70b0c24d4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459666"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/activities/{activity-id}/')
    .delete();

```