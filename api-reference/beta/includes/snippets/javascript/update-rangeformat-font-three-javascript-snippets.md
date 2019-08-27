---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c6d11d177688a4e5b7d5dc677755ab98a72f0932
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637913"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFont = {
  underline: "Single",
  color: "#FFFFFF",
  size: 26
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/font')
    .version('beta')
    .update(workbookRangeFont);

```