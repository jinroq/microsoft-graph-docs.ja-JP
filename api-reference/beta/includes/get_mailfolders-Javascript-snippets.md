---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 174d489a3e25e438d8b399e95f3832d4b947f8a6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449077"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders')
    .version('beta')
    .get();

```