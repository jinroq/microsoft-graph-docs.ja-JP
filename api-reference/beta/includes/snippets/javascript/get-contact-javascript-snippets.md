---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4cd78eed61ab4c12c61c2403bc811f854550a1e2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707539"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contacts/AAMkAGI2THk0AAA=')
    .version('beta')
    .get();

```