---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1b79b5e0b9dc602917e38eb48ce4306643efef7e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706524"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{groupId}/drive')
    .version('beta')
    .get();

```