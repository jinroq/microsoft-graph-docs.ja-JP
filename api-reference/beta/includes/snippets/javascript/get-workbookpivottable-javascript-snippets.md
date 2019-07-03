---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 750cda9395da59f9b7c216719883e2c262183445
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486059"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/root/workbook/worksheets/{id}/pivotTables/{id}')
    .version('beta')
    .get();

```