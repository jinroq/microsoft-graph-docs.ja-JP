---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 295ff960fc47fd9a6836fbaeb9a3ac5877cf48cd
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459492"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/conversations/{id}')
    .delete();

```