---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8e314bb7166460572b084c1c5f5c448d057e8837
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35472123"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/secureScores/{id}')
    .get();

```