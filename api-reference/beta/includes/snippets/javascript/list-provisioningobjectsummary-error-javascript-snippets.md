---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: faf9e3cdea25e986fc7607eb7cfc00b02496283e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720013"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/auditLogs/directoryProvisioning')
    .version('beta')
    .get();

```