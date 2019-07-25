---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6cff5b6caf4c77ccf9e65cc8cc568bf9b0cf1111
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733375"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id|userPrincipalName}/photo/$value')
    .get();

```