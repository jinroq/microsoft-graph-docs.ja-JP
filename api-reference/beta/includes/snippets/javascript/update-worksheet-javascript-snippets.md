---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f73e9750b6a177c9a7d29f333d135f1c2500abaa
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637862"
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
    .update(workbookWorksheet);

```