---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7312921fb54a9fe579bb6e29c758323e27bc3a96
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445344"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/tiIndicators')
    .version('beta')
    .get();

```