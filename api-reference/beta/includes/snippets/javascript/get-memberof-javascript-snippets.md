---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: de4951d8c8ef3a2db535146aefbaea2cbda803b5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35895561"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contacts/{id}/memberOf')
    .version('beta')
    .get();

```