---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d145ecda494e15f38190b2ccefbad8be4f914980
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637923"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTaskGroup = {
  name: "Leisure tasks"
};

let res = await client.api('/me/outlook/taskGroups')
    .version('beta')
    .post(outlookTaskGroup);

```