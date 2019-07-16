---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: af8e5a8f08a555e7791575cbeebf80a25521be3a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739894"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}')
    .get();

```