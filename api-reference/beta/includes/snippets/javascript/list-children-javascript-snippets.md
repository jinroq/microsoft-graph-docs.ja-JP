---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cfbb178b7cdb481d0db75c38292dd76929e4b159
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485965"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drives/{drive-id}/items/{item-id}/children')
    .version('beta')
    .get();

```