---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f9a3a1f6423a29dfcafe0969eb7785c78d310620
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34482214"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drives/{drive-id}/items/{item-id}/children')
    .get();

```