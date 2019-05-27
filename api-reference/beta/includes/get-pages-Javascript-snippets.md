---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ea179d374485013d5537d50b9efcc13666454240
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34435922"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/pages')
    .version('beta')
    .get();

```