---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 20d00a3a409947eb09400d19160a3f37bd62a851
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705600"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/me/classes')
    .version('beta')
    .get();

```