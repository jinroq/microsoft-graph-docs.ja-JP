---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 593f3ed6b6b821dc48fd8bd60dbbab0f208fe9d0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737965"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directory/deletedItems/microsoft.graph.group')
    .get();

```