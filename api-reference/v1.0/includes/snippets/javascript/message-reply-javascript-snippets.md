---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c50139bfa4cbb99de947ffb241f7d7eb41d28c96
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35496058"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reply = {
  comment: "comment-value"
};

let res = await client.api('/me/messages/{id}/reply')
    .post(reply);

```