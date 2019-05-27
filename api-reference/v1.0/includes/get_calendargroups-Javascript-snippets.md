---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5ddb5182449dcf083fa91a34e2ebe26d67120f8a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34479050"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendarGroups')
    .get();

```