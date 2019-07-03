---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 173f67e109d9e8cf81ebdf06f3d22aaf2bff5efc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504541"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cancel = {
  Comment: "Cancelling for this week due to all hands"
};

let res = await client.api('/me/events/{id}/cancel')
    .version('beta')
    .post(cancel);

```