---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ee2ff962a98f4a4d0cdf3b2429d9131a8da22787
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471389"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/photos')
    .get();

```