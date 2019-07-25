---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ca884fea066ef5075fedfbb579c9e07be86bb557
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712055"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/endpoints')
    .version('beta')
    .get();

```