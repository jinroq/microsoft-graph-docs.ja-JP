---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5545f1409e32a7fc718460ca14f590b839d097a9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480107"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contactFolders/{id}/contacts/delta')
    .version('beta')
    .select('displayName')
    .get();

```