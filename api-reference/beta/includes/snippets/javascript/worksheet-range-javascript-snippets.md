---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 227e6974ede1fed740a1e4e77c4862f3fed9fcd4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715960"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRange = {
  address: "address-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/Range')
    .version('beta')
    .post(workbookRange);

```