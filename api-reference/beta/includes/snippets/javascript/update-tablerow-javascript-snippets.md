---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bb5978f8c3df9be8fc795f5018d66589ffaeb097
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637886"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableRow = {
  index: 99,
  values: "values-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}')
    .version('beta')
    .update(workbookTableRow);

```