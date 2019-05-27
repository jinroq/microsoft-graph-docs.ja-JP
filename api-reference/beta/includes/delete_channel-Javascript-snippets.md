---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 3ba7f9c70f6c802000ab048a1b11c90e7f546fee
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438757"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/channels/{id}')
    .version('beta')
    .delete();

```