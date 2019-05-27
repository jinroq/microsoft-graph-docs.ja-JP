---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ca58b8a48b41c62ccef997e3c6ac14c32e63db46
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474129"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/alerts/{id}')
    .version('beta')
    .get();

```