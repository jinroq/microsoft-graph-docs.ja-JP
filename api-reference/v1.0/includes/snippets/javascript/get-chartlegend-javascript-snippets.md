---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3c2a54c3afbbac2be346ed705ada5fae683cce45
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735468"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend')
    .get();

```