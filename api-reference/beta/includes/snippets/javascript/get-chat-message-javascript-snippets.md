---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 275c4238b928bbee46d810821d944b52cfaebf29
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863579"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/chats/{id}/messages/{id}')
    .version('beta')
    .get();

```