---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d0b275e07926ca26e9d9960f3fc4c5011ea7e1ac
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717008"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const apply = {
  fields: [
    {
      key: 99,
      sortOn: "sortOn-value",
      ascending: true,
      color: "color-value",
      dataOption: "dataOption-value",
      icon: {
        set: "set-value",
        index: 99
      }
    }
  ],
  matchCase: true,
  method: "method-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/sort/apply')
    .version('beta')
    .post(apply);

```