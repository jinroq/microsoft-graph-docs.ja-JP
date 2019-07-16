---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6fb6cdff1201e9cc2e05dcf3a5905cebe96af035
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737100"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFormat = {
  columnWidth: 135,
  horizontalAlignment: "Center",
  verticalAlignment: "Center",
  rowHeight: 49,
  wrapText: false
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format')
    .update({workbookRangeFormat : workbookRangeFormat});

```