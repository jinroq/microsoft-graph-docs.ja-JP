---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4a394dac18cd92164b201fbe54ee5f3d10bb2ac5
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637982"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteSection = {
  displayName: "Section name"
};

let res = await client.api('/me/onenote/notebooks/{id}/sections')
    .version('beta')
    .post(onenoteSection);

```