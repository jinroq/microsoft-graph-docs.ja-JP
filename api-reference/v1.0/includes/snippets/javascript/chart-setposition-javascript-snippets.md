---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7c0c862109d094f2168b23ebda3fb29befceeed7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723168"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const setPosition = {
  startCell: "startCell-value",
  endCell: "endCell-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setPosition')
    .post(setPosition);

```