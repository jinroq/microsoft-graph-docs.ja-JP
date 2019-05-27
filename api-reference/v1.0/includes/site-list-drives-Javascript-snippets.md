---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a43575cee0bf173082f1e67664df9e3dfa43d2e8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34482620"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{siteId}/drives')
    .get();

```