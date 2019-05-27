---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6882a43d76f30f7f56d440be56668e8b9c588686
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34458015"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains/{domain-name}/verify')
    .post();

```