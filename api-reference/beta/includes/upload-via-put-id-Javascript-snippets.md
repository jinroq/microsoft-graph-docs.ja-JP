---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 056f1bb68586a9b5846bf2e03b1ed68aea7419b5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465868"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const Stream = The contents of the file goes here.;

let res = await client.api('/me/drive/items/{item-id}/content')
    .version('beta')
    .put({Stream : Stream});

```