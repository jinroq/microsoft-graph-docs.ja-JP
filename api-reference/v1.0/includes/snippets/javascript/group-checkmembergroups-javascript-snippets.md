---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 81c580e4a4e19c51ecb0ce6056b6916655b3929e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740186"
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

let res = await client.api('/groups/{id}/checkMemberGroups')
    .post(String);

```