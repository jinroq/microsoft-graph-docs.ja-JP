---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cffc768a17ba60e652efa224acf4963b0b5bc7fa
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449539"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/transitiveMembers')
    .version('beta')
    .get();

```