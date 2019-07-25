---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 89ce97b586aee6a805c2e40f9f65be6955ff17f8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35865079"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendar/events')
    .version('beta')
    .get();

```