---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 974543c57556c98a784270b3d3abbba62c6bbf07
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723596"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookWorksheet = {
  position: 99,
  name: "name-value",
  visibility: "visibility-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}')
    .version('beta')
    .update({workbookWorksheet : workbookWorksheet});

```