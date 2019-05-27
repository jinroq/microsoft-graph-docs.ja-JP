---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: efe03965de2a0b2affdfa1f271d972c13dd5c87d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34468634"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/createdObjects')
    .get();

```