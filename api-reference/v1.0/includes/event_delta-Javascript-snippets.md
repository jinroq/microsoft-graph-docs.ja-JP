---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 373337d7a5b296ff89efe7c0f3f88f97714cac5b
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536422"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendarView/delta?startdatetime=%7Bstart_datetime%7D&enddatetime=%7Bend_datetime%7D')
    .get();

```