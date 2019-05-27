---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 61505fde2fefa4eb2beb40550bc2aa6c79609bbe
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34466064"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{siteId}/drives')
    .version('beta')
    .get();

```