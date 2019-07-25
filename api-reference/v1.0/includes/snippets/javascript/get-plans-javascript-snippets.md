---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d3d42929f6d53c7cdbe3ef91637022cf5d8a862e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730143"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/planner/plans')
    .get();

```