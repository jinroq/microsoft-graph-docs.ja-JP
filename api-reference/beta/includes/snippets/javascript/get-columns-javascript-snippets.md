---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c5146959d51be22b369ae0ec68b786834f44712e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717220"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns')
    .version('beta')
    .skip(5)
    .top(5)
    .get();

```