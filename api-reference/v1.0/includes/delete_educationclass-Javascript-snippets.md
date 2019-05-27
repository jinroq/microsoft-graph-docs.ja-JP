---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d82df24336f40a7f0c89218aeb3c9acee14fb6c8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459180"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/{class-id}')
    .delete();

```