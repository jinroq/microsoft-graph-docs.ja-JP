---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d8bd2f45de0b5ad816a5d459eee327b52d39e450
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732085"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/AAMkADhAAAW-VPeAAA=/')
    .select('internetMessageHeaders')
    .get();

```