---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 749f7edfebb38b0e3ef34df6aa12b0bfdc8aea7f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447111"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/programControlTypes')
    .version('beta')
    .get();

```