---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 36de14757c69b0610701e2a795c23c72164d04ad
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858357"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/owners')
    .version('beta')
    .get();

```