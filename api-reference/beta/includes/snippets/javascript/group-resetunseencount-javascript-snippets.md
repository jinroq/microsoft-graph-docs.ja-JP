---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f4a94b12db2601efbf5ff3cfec81b485bb5f4900
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713537"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/resetUnseenCount')
    .version('beta')
    .post();

```