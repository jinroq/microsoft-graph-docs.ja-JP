---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c6c2aa567c85d1b48c343b0b8c7953dd9ce7ec69
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726604"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getTeamsDeviceUsageUserCounts(period='D7')')
    .version('beta')
    .get();

```