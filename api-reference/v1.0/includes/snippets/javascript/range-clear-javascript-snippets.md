---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3b674fa5a3274d3f03f37c3ee178d847a46ec67e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736066"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const clear = {
  applyTo: "applyTo-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/clear')
    .post(clear);

```