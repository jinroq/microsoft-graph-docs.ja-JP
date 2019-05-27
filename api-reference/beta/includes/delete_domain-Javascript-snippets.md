---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: af3bb08b5a35275970f92aafb7a4e10d97ffc697
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438505"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains/contoso.com')
    .version('beta')
    .delete();

```