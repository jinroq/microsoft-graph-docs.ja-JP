---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8d85bd1d682dd5c28465c4814141fa97692905cb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504547"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drives')
    .version('beta')
    .get();

```