---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fedfe76fee1e7b3b970f67df8529bb3d115b3a89
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730626"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTaskGroup = {
  name: "Personal Tasks",
};

let res = await client.api('/me/outlook/taskgroups/AAMkADIyAAAhrbe-AAA=')
    .version('beta')
    .update({outlookTaskGroup : outlookTaskGroup});

```