---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ed037660bde9478d01343fdd402ee85fa3743477
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471666"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/children')
    .expand('thumbnails')
    .get();

```