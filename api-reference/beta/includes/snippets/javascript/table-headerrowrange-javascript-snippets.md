---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d421e4014f77874e5bac88c03590511348cfb41d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485603"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/HeaderRowRange')
    .version('beta')
    .post();

```