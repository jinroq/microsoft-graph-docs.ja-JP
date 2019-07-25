---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 381cca61cccff66f1a73a67f14f97727ea827a0c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706685"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryRole = {
  description: "description-value",
  displayName: "displayName-value",
  roleTemplateId: "roleTemplateId-value"
};

let res = await client.api('/directoryRoles')
    .version('beta')
    .post({directoryRole : directoryRole});

```