---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 179fd29af5d2ae7361e0a990b4e50553ddd179e3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35487173"
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

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/font')
    .version('beta')
    .update({workbookRangeFont : workbookRangeFont});

```