---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8b2c75d9d5ee6275448a69892d3ea42fee16f4ef
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34466303"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/transitiveMembers')
    .get();

```