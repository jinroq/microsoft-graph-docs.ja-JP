---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 35732ba3864b75624d169cb1e14fc2a639031e0c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527449"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/subscriptions/{id}')
    .version('beta')
    .get();

```