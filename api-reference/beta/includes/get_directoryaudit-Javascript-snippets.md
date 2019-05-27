---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f5be1b5195cfdd9fd07ec14232d9d664565a4d46
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472084"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/auditLogs/directoryAudits/{id}')
    .version('beta')
    .get();

```