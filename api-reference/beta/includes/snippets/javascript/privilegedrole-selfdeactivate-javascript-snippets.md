---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5b779729db4d53f2cdc99b1f4c6a0b2b1cc81578
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486246"
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