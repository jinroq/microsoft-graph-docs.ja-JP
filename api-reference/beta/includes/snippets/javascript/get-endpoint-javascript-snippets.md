---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 191ec0b1d2a6103c3b3b1e6708fcb1f6d19d5721
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712295"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/endpoints/{id}')
    .version('beta')
    .get();

```