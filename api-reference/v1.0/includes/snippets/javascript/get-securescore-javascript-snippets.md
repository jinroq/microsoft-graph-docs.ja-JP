---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8e314bb7166460572b084c1c5f5c448d057e8837
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731829"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/secureScores/{id}')
    .get();

```