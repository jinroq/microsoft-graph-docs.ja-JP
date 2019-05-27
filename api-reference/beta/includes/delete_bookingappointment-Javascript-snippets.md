---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fa84be07490f9f1962f25640ec8d5d87d01a0685
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438946"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKqAAA=')
    .version('beta')
    .delete();

```