---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ecd5f1a44578abdb95379dbe09c4746f7c15ca9a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448035"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=')
    .version('beta')
    .get();

```