---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1d0d2c2b32642fc16be00f4523328a0b283ce649
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740678"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/totalRowRange')
    .post();

```