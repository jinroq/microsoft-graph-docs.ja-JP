---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b0fe630be99028d4983e0fc0f2ea9a11d24f426b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720921"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTask = {
  dueDateTime:  {
      dateTime: "2016-05-06T16:00:00",
      timeZone: "Eastern Standard Time"
  }
};

let res = await client.api('/me/outlook/tasks/AAMkADA1MTHgwAAA=')
    .version('beta')
    .update({outlookTask : outlookTask});

```