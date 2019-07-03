---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4d6fab2e52b09d3042552d4d9b682874782a7110
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526352"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish')
    .version('beta')
    .post();

```