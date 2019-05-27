---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fff8f1544a2800be7bb98247403d1c415594ac05
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474948"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/calendarView')
    .version('beta')
    .get();

```