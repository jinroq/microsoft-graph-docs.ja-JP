---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1d2436476e8abb7cb4afb2444a4cabcb5678f810
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486725"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}')
    .version('beta')
    .get();

```