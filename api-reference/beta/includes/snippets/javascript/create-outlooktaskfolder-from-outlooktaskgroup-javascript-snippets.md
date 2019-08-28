---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a668fc0b3f92c54060b69568b92826890b0e87f5
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633665"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const taskfolders = {
  name: "Cooking"
};

let res = await client.api('/me/taskgroups/AAMkADIyAAAhrbe-AAA'/taskfolders')
    .version('beta')
    .post(taskfolders);

```