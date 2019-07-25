---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f90c18bfe0495d9e8770c9dc977943a20a2a363e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35725108"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/subscriptions/{id}')
    .version('beta')
    .delete();

```