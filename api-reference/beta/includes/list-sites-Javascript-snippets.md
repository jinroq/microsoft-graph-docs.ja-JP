---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: daceffe89c908f9bfb6562b8f3ec57dc6e817499
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444399"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites')
    .version('beta')
    .filter('siteCollection/root ne null')
    .get();

```