---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ee2ff962a98f4a4d0cdf3b2429d9131a8da22787
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736011"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/photos')
    .get();

```