---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0ef19d9b84f1d6921e31f20364684022ebddabb1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731870"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sectionGroup = {
  displayName: "Section group name"
};

let res = await client.api('/me/onenote/sectionGroups/{id}/sectionGroups')
    .post({sectionGroup : sectionGroup});

```