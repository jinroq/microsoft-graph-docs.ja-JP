---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ca58b8a48b41c62ccef997e3c6ac14c32e63db46
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710487"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/alerts/{id}')
    .version('beta')
    .get();

```