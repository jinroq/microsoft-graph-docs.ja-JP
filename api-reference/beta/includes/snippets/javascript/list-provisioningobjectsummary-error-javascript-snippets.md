---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: faf9e3cdea25e986fc7607eb7cfc00b02496283e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35484944"
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