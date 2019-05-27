---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 71043814d9b930ebc10679fd7c0d0ebc71c203cc
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449112"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/AAMkAGVmMDEzM')
    .version('beta')
    .get();

```