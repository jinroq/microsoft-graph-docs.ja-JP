---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fe24d18c0dcc23884c36b07762ff14c6d21b182e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729380"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sectionGroup = {
  displayName: "Section group name"
};

let res = await client.api('/me/onenote/notebooks/{id}/sectionGroups')
    .version('beta')
    .post({sectionGroup : sectionGroup});

```