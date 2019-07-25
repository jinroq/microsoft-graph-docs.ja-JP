---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2a29dc08dfc7b80e551a3130a591e069417a1713
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856144"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendars')
    .version('beta')
    .get();

```