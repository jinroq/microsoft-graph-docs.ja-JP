---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6c16312150474dfcfeee514354baf46c2019f09c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737829"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFont = {
  italic: true,
  size: 26
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$B$1')/format/font')
    .update({workbookRangeFont : workbookRangeFont});

```