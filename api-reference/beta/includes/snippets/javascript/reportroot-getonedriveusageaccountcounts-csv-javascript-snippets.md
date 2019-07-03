---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 13700ceaccecf1f9507f316c95637a28173c3346
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527715"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOneDriveUsageAccountCounts(period='D7')')
    .version('beta')
    .get();

```