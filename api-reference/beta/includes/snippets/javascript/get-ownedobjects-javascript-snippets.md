---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c3f252b5a49dd6cd1ea611a47e6f769b96ee965c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724037"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/ownedObjects')
    .version('beta')
    .get();

```