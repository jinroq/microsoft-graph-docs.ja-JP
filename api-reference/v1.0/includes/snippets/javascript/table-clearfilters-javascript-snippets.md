---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cc7e078ae1e8d01eb310de3789c12e0fd05c30e3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738305"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/clearFilters')
    .post();

```