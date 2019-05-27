---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f8a20e9595a24006fa5c006e4ede9cc966219f08
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34478140"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{groupId}/drives')
    .get();

```