---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b6682a34f9226e32e9eac1953ddf339ade8737b4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724085"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages')
    .version('beta')
    .select('sender,subject')
    .get();

```