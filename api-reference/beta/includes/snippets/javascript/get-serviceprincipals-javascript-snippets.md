---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 438730c3efb2fc172c2fa31d7f92a7dc0ffae261
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485433"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals')
    .version('beta')
    .get();

```