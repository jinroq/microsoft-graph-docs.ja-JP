---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a9d39c395c66d44326eb600a2ab92963ec448db9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721097"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  groupIds: [
    "groupIds-value"
  ]
};

let res = await client.api('/contacts/{id}/checkMemberGroups')
    .version('beta')
    .post(String);

```