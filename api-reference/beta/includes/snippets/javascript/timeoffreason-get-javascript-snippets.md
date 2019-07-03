---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5b64273de56472cfadadb3c13decf7fb3fc66529
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527552"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}')
    .version('beta')
    .get();

```