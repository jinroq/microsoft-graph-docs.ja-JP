---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a2d86e716a423ed128ed2a5f7ee75e4130a10327
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469979"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/alerts')
    .get();

```