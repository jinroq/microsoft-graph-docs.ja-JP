---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2f6100df948bed777cff84b9f151585c727a9c5f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728807"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTaskGroup = {
  name: "Leisure tasks"
};

let res = await client.api('/me/outlook/taskGroups')
    .version('beta')
    .post({outlookTaskGroup : outlookTaskGroup});

```