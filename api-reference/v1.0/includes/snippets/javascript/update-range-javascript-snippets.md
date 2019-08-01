---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 53c2a4d539f10f1902eaf761af3c840da5290e0b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733857"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRange = {
"values" : [["Hello", "100"],["1/1/2016", null]],
"formula" : [[null, null], [null, "=B1*2"]],
"numberFormat" : [[null,null], ["m-ddd", null]]
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='A1:B2')')
    .update(workbookRange);

```