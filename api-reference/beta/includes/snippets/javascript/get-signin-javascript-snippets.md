---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fcb2eb5b2d80604694f7d8321907ade6799f69a2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717639"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/auditLogs/signIns/{id}')
    .version('beta')
    .get();

```