---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: aea6bdfbc04e7b8e564dd489632ed0d90829bfbb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35496051"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range')
    .post();

```