---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 663077ea71383a76e28c0ad8c14baa253b408282
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735930"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/entireColumn')
    .get();

```