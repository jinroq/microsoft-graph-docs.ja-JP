---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d78dd342594f9b7f014c90586de47ef9efcd05c5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724920"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/synchronization/templates')
    .version('beta')
    .get();

```