---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d29edbb02d510c1c8440f4337cc3813c59eca3cd
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442593"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/autofitRows')
    .version('beta')
    .post();

```