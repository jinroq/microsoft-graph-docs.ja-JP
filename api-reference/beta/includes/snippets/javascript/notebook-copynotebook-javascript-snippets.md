---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fa8c97bb3b2ec83f64192536f0f099b262c8e346
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527406"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteOperation = {
  groupId: "groupId-value",
  renameAs: "renameAs-value"
};

let res = await client.api('/me/onenote/notebooks/{id}/copyNotebook')
    .version('beta')
    .post(onenoteOperation);

```