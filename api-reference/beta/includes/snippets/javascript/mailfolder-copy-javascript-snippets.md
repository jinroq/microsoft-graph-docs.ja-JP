---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 195be5614c6a364c4b2d474280847d70b7f491c0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485510"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  destinationId: "destinationId-value"
};

let res = await client.api('/me/mailFolders/{id}/copy')
    .version('beta')
    .post(mailFolder);

```