---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fcc4965903ea27c02f59dc65688dab46a117ae17
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34470621"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/headerRowRange')
    .post();

```