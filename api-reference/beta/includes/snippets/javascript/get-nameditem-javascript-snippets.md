---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 86efc52ecf3f329f631cbefb8a9ebe8875796a12
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486380"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}')
    .version('beta')
    .get();

```