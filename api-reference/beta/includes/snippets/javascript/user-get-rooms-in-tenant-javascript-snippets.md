---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ab52f9899b1df42a3adeb2c72b17f844b2b0fbfb
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716668"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/findRooms')
    .version('beta')
    .get();

```