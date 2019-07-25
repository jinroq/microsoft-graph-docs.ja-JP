---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c56cc4e70ae3a7024732f06ac19b7fd845208a38
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709584"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish')
    .version('beta')
    .post();

```