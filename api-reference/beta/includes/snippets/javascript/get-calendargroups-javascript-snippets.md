---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3874501ecd3b5c90e8cb0a6ebbc428c479f10d70
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35484968"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendarGroups')
    .version('beta')
    .get();

```