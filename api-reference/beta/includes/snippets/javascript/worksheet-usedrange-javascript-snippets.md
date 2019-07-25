---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 26f462438b3f5a50c47472c80c243c668c1f9c46
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715917"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/UsedRange(valuesOnly=true)')
    .version('beta')
    .get();

```