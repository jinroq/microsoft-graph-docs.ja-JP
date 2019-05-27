---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ffc2c789757ef59679644fdac846a9d3a05926c3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34478217"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}')
    .get();

```