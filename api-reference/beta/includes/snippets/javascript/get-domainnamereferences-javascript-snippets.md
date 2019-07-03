---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 300aa93262e375366c3b9a400fb9f63c4c3c8874
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504578"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains/contoso.com/domainNameReferences')
    .version('beta')
    .get();

```