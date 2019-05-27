---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 76646b569e9c45480d0ac67ff5e62f5c2c9c48f3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444189"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/delta')
    .version('beta')
    .get();

```