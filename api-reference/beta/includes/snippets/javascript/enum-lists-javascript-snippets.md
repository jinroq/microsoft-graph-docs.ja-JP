---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6abbf8d8627ec46add62c89547fd4d7dbfaf3f8d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504544"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists')
    .version('beta')
    .get();

```