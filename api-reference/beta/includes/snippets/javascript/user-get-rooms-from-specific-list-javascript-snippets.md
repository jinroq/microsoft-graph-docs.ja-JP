---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 07798bf2ea25e036430f6a4e22edbc203ed91ffe
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716665"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/findRooms(RoomList='Building2Rooms@contoso.onmicrosoft.com')')
    .version('beta')
    .get();

```