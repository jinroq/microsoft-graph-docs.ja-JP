---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4fe643ea37c01f738576f0473ccf0a18676359e4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709739"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/bookingBusinesses/Fabrikam@M365B489948.onmicrosoft.com')
    .version('beta')
    .get();

```