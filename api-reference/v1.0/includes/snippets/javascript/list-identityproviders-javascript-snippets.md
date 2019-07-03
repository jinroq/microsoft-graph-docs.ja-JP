---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 44fa434585498096699c2011d1129f9ec3991676
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35496085"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityProviders')
    .get();

```