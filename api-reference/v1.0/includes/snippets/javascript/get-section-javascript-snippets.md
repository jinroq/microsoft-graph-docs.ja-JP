---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 72e71a3dec0f4f02a7fbee1e869eb7407c24e8f3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35513703"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/sections/{id}')
    .get();

```