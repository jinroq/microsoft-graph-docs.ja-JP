---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 624517e7f1bff2c07e29277e2ad8e3c734f5c6ed
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711989"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/members')
    .version('beta')
    .get();

```