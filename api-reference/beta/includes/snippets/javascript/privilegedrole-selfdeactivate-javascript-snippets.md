---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5b779729db4d53f2cdc99b1f4c6a0b2b1cc81578
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728541"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoles/{id}/selfDeactivate')
    .version('beta')
    .post();

```