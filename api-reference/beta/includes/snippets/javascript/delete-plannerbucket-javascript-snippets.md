---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1abbf9a9de03b976ec4f3afaefaba04043ec83d7
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413489"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/buckets/{id}')
    .version('beta')
    .delete();

```