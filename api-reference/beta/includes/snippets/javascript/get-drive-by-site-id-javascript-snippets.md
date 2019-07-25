---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2988460caff6334ebf137ee903665eee3b34d5e1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706531"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{siteId}/drive')
    .version('beta')
    .get();

```