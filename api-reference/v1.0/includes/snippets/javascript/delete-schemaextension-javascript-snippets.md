---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6b7e32087895b59336fb3894d3c9ce250037b856
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722217"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/schemaExtensions/{id}')
    .delete();

```