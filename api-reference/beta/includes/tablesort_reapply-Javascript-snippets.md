---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f767bf9504d3d49351b87a3be8714999bd47a9e4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469414"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/sort/reapply')
    .version('beta')
    .post();

```