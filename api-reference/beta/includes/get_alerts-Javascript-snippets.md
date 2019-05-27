---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fc3e8b106e3e2cdbee3005dce26af2d97a2df475
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474101"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/alerts')
    .version('beta')
    .get();

```