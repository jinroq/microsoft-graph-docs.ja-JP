---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c8c326c1e7bb7d83680fbe4ef2568b205deb8551
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35513747"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/plans/{plan-id}/buckets')
    .get();

```