---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 10469783cfb156c2bd21eaf80194b07ed0780a5c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720860"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/masterCategories')
    .version('beta')
    .get();

```