---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e1ccd54b07b8b847d331dab8f6ca27fb4bc54aae
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526730"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeBorder = {
  index: {
  }
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/borders/ItemAt')
    .version('beta')
    .post({workbookRangeBorder : workbookRangeBorder});

```