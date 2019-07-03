---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7c4fb278ff0dd9e052303b0ad4db2e638308e275
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35487210"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/EntireColumn')
    .version('beta')
    .get();

```