---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 60e0f227c16044dd6c7790bd78966dafcbf573c0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446943"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/AAMkAGE1M88AADUv0uAAAG=/attachments/AAMkAGE1Mg72tgf7hJp0PICVGCc0g=')
    .version('beta')
    .get();

```