---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d5f8ddb3e5c3dadf91625304cbcf6c672b19cbea
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710422"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications/{id}')
    .version('beta')
    .delete();

```