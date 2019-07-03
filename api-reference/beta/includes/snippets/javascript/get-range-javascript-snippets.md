---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5fa9271110e386c2d906a1b1b8c6274850e8b700
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35487048"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range')
    .version('beta')
    .get();

```