---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a59707d81fe3fd08338365eaba83a9caeb59ee5e
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637797"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directorySetting = {
  values: [
    {
      name: "name-value",
      value: "value-value"
    }
  ]
};

let res = await client.api('/settings/{id}')
    .version('beta')
    .update(directorySetting);

```