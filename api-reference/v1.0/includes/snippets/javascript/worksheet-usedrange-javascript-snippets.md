---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6f77d6932984be128a35a11bb36f7cad76da16ba
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736817"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange')
    .get();

```