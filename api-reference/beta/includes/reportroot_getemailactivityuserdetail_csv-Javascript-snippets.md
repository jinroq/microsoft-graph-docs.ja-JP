---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d4f97c03391cbdacb9fc35057eb4065002516835
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442313"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getEmailActivityUserDetail(period='D7')')
    .version('beta')
    .get();

```