---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8fd66bd2e493bb3ef6febb74a556e2f6a1fdd964
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719069"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointActivityUserCounts(period='D7')')
    .version('beta')
    .get();

```