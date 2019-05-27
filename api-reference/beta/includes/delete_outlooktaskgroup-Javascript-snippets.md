---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: aa6b65bbfbc0ef5b9ee05016e712bf3c82d1ce45
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437798"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/taskgroups/AAMkADIyAAAhrbe-AAA=')
    .version('beta')
    .delete();

```