---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6ffaead5aed0eb070e370a2099aa442197e70f8e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35882374"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendarGroups/{id}/calendars')
    .get();

```