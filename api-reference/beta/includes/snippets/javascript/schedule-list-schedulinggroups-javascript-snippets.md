---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fca735f841ba58d39cfc875bdbf30f6754c53c7c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718233"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule/schedulingGroups')
    .version('beta')
    .get();

```