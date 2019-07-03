---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 385e568a1e25b0c947a32792627cad2ad392aad2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35513395"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFont = {
  bold: true,
  color: "#4B180E",
  size: 26
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$A$1')/format/font')
    .update({workbookRangeFont : workbookRangeFont});

```