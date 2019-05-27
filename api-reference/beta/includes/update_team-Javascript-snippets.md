---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fc650bf378e38a9acae85cd8c433a7fb07c03742
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475872"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
  memberSettings: {
    allowCreateUpdateChannels: true
  },
  messagingSettings: {
    allowUserEditMessages: true,
    allowUserDeleteMessages: true
  },
  funSettings: {
    allowGiphy: true,
    giphyContentRating: "strict"
  }
};

let res = await client.api('/teams/{id}')
    .version('beta')
    .update({team : team});

```