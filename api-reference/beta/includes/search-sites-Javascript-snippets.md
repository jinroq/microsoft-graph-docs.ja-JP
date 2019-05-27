---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3e2c3e0d5c001963e04cf8a079a3db8a47a76125
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480401"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites')
    .version('beta')
    .get();

```