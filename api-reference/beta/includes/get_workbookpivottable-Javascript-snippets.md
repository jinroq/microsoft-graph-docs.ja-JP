---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 750cda9395da59f9b7c216719883e2c262183445
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445071"
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