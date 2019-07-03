---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 10469783cfb156c2bd21eaf80194b07ed0780a5c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504633"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/masterCategories')
    .version('beta')
    .get();

```