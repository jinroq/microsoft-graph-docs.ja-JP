---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: df16d55be836c7cea323f143396ca84f258788d4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720292"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoles/{id}/assignments')
    .version('beta')
    .get();

```