---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 743f327c4adaef1f47eddc4d218f8335eb08bb17
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739081"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}')
    .delete();

```