---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2988460caff6334ebf137ee903665eee3b34d5e1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35503864"
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