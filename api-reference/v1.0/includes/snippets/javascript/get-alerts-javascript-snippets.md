---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a2d86e716a423ed128ed2a5f7ee75e4130a10327
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35496034"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/alerts')
    .get();

```