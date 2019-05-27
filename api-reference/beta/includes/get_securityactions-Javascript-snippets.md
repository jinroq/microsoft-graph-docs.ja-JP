---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b32a87d85c4b35651c175ed06713221d1a3bc972
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446275"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/securityActions')
    .version('beta')
    .get();

```