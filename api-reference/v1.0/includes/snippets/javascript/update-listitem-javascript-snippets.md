---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bc0cffd2dc6f8423995c127bdd0264d83867c7d5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731431"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const fieldValueSet = {
    Color: "Fuchsia",
    Quantity: 934
};

let res = await client.api('/sites/{site-id}/lists/{list-id}/items/{item-id}/fields')
    .update({fieldValueSet : fieldValueSet});

```