---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9f25d0e2d334fdc80f83c6d276519b0d7968ef5d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728012"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFill = {
  color: "#FF0000"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/fill')
    .version('beta')
    .update({workbookRangeFill : workbookRangeFill});

```