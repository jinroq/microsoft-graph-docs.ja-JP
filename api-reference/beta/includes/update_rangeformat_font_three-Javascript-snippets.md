---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 54fef5e5dad9790039922ee9769d522a2c615748
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461658"
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
    .update({workbookRangeFont : workbookRangeFont});

```