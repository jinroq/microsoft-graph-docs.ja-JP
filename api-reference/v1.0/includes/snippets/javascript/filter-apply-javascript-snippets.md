---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5c097359bb725086865516a532602ea4f7fe009a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740292"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const apply = {
  criteria: {
    criterion1: "criterion1-value",
    criterion2: "criterion2-value",
    color: "color-value",
    operator: {
    },
    icon: {
      set: "set-value",
      index: 99
    },
    dynamicCriteria: "dynamicCriteria-value",
    values: {
    },
    filterOn: "filterOn-value"
  }
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/filter/apply')
    .post(apply);

```