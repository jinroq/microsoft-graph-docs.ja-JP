---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: de4951d8c8ef3a2db535146aefbaea2cbda803b5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448979"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contacts/{id}/memberOf')
    .version('beta')
    .get();

```