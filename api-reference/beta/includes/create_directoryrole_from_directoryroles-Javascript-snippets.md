---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 381cca61cccff66f1a73a67f14f97727ea827a0c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34481122"
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