---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fb25f1360fe346df752e93ab70375326fcc7c83d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724162"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/joinedTeams')
    .version('beta')
    .get();

```