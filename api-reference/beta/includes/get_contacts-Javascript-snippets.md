---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 49c0bea4151147a5d9bc07a4539214184e092f54
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472540"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contacts')
    .version('beta')
    .select('displayName,emailAddresses')
    .get();

```