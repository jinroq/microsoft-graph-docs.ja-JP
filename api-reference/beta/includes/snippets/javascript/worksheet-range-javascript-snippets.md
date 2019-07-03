---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 227e6974ede1fed740a1e4e77c4862f3fed9fcd4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486516"
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