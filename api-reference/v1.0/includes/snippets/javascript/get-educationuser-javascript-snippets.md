---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e232e352fc245a8739ecc9543f77a11e4ccb7835
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35732710"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/users/{user-id}')
    .get();

```