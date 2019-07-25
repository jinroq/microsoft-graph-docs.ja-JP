---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6ed7779e22fbc5452d7d6b2adc0963855ecf232e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721902"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drives/{drive-id}/items/{item-id}/analytics')
    .version('beta')
    .get();

```