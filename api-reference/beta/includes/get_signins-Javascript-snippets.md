---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 27ec6610634a2266c765361183657e87a9c1874d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446002"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/auditLogs/signIns')
    .version('beta')
    .get();

```