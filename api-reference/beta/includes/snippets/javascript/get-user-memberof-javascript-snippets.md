---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3dfa5d99c2a3e48237dddafa3f7b563c95109d80
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707111"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/memberOf')
    .version('beta')
    .get();

```