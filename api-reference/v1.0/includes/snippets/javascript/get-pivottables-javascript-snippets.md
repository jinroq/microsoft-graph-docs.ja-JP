---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3c3392836fbef1a3ea2e4e07270db614d3ac1341
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740419"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/workbook/worksheets/{id}/pivotTables')
    .get();

```