---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 244d98fdea30fd3a6b3a22130fceb3b0d120f354
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737840"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFill = {
  color: "#0000FF"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$C$1')/format/fill')
    .update({workbookRangeFill : workbookRangeFill});

```