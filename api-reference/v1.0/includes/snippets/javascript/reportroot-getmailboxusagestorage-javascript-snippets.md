---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4488ae9b931f959119643b6a46aaa93d557f27fb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35513317"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getMailboxUsageStorage(period='D7')')
    .get();

```