---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5db7c0b4505753d54dab1c689f7b443999f41aca
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34466789"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/DataBodyRange')
    .version('beta')
    .post();

```