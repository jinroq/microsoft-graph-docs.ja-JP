---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a8262be592fc3cdf9ba98bbe5ce5e483319bdbbd
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709385"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookingService = {
    @odata.type:"#microsoft.graph.bookingService",
    defaultDuration:"PT30M"
};

let res = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976')
    .version('beta')
    .update({bookingService : bookingService});

```