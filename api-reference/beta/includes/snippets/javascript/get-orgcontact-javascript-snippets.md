---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 82fc62d301155f5fe1b31b3ecf2e1b899dfbea0d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35525973"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contacts/{id}')
    .version('beta')
    .get();

```