---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d6f0a5730e14a2620afdbc6f51630a89119da8d7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34477615"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages')
    .select('sender,subject')
    .get();

```