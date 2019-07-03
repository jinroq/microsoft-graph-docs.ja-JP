---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fd94bb2451548b0033e892bbfc2c382d10482fe7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35495854"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableColumn = {
  index: 3,
  values: [
    {
    }
  ]
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/add')
    .post(workbookTableColumn);

```