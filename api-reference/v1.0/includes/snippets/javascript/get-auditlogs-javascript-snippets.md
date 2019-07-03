---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6f5248c02279365f57e91cf85670b963e8e618b1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471143"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/auditLogs')
    .get();

```