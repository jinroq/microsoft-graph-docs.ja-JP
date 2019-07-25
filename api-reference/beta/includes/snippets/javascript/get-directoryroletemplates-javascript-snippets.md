---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ff48ecd82c2db246e48a8794a032d4301f7627dc
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713333"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoleTemplates')
    .version('beta')
    .get();

```