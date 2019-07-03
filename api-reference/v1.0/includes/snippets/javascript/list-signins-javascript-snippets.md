---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f6bf1bcbc9767c9212ac1e15b5d3344351910928
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35496083"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/auditLogs/signIns')
    .get();

```