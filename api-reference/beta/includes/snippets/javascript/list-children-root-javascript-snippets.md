---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7c37218459ae43302ae2b2462031317843d278bb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526901"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/children')
    .version('beta')
    .get();

```