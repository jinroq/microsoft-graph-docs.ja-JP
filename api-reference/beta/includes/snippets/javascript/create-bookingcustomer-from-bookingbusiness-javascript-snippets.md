---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3ac4504c7438d00d9c62853d39cb07594c95020f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527747"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const bookingCustomer = {
    displayName: "Joni Sherman",
    emailAddress: "jonis@relecloud.com"
};

let res = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers')
    .version('beta')
    .post({bookingCustomer : bookingCustomer});

```