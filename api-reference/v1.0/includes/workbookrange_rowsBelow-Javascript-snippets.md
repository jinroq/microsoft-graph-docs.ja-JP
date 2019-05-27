---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8a4df57dac0991a176e810541ae613e611ddcad3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34450511"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)')
    .post();

```