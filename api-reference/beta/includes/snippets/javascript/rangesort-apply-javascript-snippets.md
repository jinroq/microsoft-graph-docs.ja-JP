---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6ef57b2d5d64dc2f4d01d9918fe59bf38609adc7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719751"
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
  hasHeaders: true,
  orientation: "orientation-value",
  method: "method-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/sort/apply')
    .version('beta')
    .post(apply);

```