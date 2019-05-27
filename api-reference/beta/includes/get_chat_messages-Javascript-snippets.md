---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 29e3d31f41e254305010aa4a211e3335bc62f7e0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472778"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/chats/{id}/messages')
    .version('beta')
    .get();

```