---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e5e3a7c5022e231c191f35e30ddf87fbac590605
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457938"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/subscriptions/socketIo')
    .get();

```