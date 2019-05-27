---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5341f88326a350423c94835c6a474f90927a20fa
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446380"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/sectionGroups/{id}')
    .version('beta')
    .get();

```