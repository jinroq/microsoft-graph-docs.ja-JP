---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f8cb1f2e23b095557abd15ad53fd4d6e1506aa78
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486060"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/application')
    .version('beta')
    .get();

```