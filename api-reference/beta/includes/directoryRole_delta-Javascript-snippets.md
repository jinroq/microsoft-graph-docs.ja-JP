---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5636d2cd92bb4c0ca47707980ac348e3d8932f82
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437280"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoles/delta')
    .version('beta')
    .get();

```