---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 03a08f1b39d02ffe9162013cd693ba248b86f7a9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504159"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const Boolean = {
  groupId: "ffffffff-ffff-ffff-ffff-ffffffffffff"
};

let res = await client.api('/groupLifecyclePolicies/renewGroup')
    .version('beta')
    .post(Boolean);

```