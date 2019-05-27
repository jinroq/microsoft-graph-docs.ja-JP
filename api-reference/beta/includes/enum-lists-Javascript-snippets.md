---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6abbf8d8627ec46add62c89547fd4d7dbfaf3f8d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436804"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists')
    .version('beta')
    .get();

```