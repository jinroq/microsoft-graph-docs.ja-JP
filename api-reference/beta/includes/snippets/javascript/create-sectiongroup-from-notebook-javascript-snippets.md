---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fe24d18c0dcc23884c36b07762ff14c6d21b182e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35487239"
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