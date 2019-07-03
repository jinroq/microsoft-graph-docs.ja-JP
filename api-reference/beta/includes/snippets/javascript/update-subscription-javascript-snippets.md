---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1fb08ef1da9d09df8fc8fd1a18f09507814b7e96
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35487081"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const subscription = {
   expirationDateTime:"2016-11-22T18:23:45.9356913Z"
};

let res = await client.api('/subscriptions/{id}')
    .version('beta')
    .update({subscription : subscription});

```