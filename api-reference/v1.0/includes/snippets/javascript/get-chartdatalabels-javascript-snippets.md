---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 35c7937273b9443982d0ddb6dd76f25b3f6f9d4c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735701"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/dataLabels')
    .get();

```