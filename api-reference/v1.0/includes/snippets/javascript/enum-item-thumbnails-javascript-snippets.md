---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a2b07768fbefac5455f6f2d4b7bcf5075256b38a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35514555"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/thumbnails')
    .get();

```