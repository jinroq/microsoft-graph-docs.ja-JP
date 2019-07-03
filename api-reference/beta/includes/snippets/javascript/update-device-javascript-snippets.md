---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 324d0ba94693ad9c39cab2e20b63baf30950ed5f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486026"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const device = {
  accountEnabled: false
};

let res = await client.api('/devices/{id}')
    .version('beta')
    .update({device : device});

```