---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f6bf1bcbc9767c9212ac1e15b5d3344351910928
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734091"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/auditLogs/signIns')
    .get();

```