---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 43915ed94ba5ba944e634d99c31a084fe76935b9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34455015"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drives/{drive-id}')
    .get();

```