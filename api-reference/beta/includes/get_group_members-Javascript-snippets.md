---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 624517e7f1bff2c07e29277e2ad8e3c734f5c6ed
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471034"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/members')
    .version('beta')
    .get();

```