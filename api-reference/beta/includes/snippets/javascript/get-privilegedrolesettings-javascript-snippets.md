---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5087a5d06c8c5c28dde639bc1bb48af555b128d9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728413"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoles/{id}/settings')
    .version('beta')
    .get();

```