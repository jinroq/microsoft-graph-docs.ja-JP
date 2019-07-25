---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 753f72d2ff458eeb8795e9d3ce361267636594f3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706422"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/settings')
    .version('beta')
    .get();

```