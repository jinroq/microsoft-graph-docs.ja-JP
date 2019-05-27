---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3834552430883e6045556158e0960d859f3b9f89
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457790"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendarView/delta')
    .get();

```