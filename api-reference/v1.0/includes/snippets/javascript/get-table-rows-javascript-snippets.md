---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0abb3f997dffb514c231de849b334bf44ebb9924
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723029"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows')
    .skip(5)
    .top(5)
    .get();

```