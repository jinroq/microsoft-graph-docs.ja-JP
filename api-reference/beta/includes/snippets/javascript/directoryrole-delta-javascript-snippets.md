---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5636d2cd92bb4c0ca47707980ac348e3d8932f82
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713419"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoles/delta')
    .version('beta')
    .get();

```