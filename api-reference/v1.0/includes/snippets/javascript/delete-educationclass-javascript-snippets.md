---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d82df24336f40a7f0c89218aeb3c9acee14fb6c8
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739969"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/{class-id}')
    .delete();

```