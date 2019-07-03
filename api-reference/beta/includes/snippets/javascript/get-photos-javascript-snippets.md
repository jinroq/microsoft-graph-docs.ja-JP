---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e8443f1d294d01cb7fa7f9e742007534858d23f3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526458"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/photos')
    .version('beta')
    .get();

```