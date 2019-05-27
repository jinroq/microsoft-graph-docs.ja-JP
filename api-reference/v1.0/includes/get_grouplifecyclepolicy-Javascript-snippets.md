---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 63a3f59d6dd4323d7ec3ddf81a84a9967d4e7824
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34476425"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groupLifecyclePolicies')
    .get();

```