---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d421e4014f77874e5bac88c03590511348cfb41d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724835"
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