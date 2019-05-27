---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 101e6b522909a2c7ab66c53a7149c6487612f55b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446478"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoles/{id}/scopedMembers')
    .version('beta')
    .get();

```