---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e09b7740e60fd71fd9adf6c9c2fd7f3498af3820
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474549"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}')
    .version('beta')
    .get();

```