---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: dfdb4fecdca336d69e9d8f247bf213a712d21553
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35503805"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices/{id}/transitiveMemberOf')
    .version('beta')
    .get();

```