---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0b11d0da72abb33c4fd42f707f227bbaab6becce
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459534"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendarGroups/{id}')
    .delete();

```