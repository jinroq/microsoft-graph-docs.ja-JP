---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 09be6cce37496400b52c3e4798f2d33113feec0b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438050"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}')
    .version('beta')
    .delete();

```