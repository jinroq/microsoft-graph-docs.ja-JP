---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f2f02d6de30260f6c6947f0704ffa92590722f50
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724708"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}')
    .version('beta')
    .get();

```