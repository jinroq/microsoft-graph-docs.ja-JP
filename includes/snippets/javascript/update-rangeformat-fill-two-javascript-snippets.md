---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 84702141240a051f4f64ca8763cb20539f1725f2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35533564"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFill = {
  color: "#00FF00"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/fill')
    .update({workbookRangeFill : workbookRangeFill});

```