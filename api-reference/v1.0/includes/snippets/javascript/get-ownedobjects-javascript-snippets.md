---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 586925743f98706667483bd2a4a39c91d447a3be
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734292"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/ownedObjects')
    .get();

```