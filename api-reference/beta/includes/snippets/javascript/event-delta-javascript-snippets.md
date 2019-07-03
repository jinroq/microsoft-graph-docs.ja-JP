---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 918d73c1863df00e4b4f473a154ae77d6b17b232
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504536"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendarview/delta?startdatetime=%7Bstart_datetime%7D&enddatetime=%7Bend_datetime%7D')
    .version('beta')
    .get();

```