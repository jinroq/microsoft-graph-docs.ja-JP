---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c66e58148c4a830d436169401033698340eb10be
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34473422"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendarView')
    .get();

```