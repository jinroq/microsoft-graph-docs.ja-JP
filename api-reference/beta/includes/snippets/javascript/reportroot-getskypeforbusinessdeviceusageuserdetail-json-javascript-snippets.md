---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c3b4ef413d279d21fb696f8bad15e2495b223021
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527911"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')')
    .version('beta')
    .get();

```