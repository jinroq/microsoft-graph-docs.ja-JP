---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e656d4ca4342ec99e3c58e43bd2fa65ec0bd51b0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858408"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/memberOf')
    .version('beta')
    .get();

```