---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9cddbe34e9d477a846a934f828882d0af125e8e3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504090"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows')
    .version('beta')
    .skip(5)
    .top(5)
    .get();

```