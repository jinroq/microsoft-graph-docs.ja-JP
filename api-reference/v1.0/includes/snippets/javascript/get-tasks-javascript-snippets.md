---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 510e638ace69a6dfbe7cad8332a38f0718d6c0a3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730034"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/planner/tasks')
    .get();

```