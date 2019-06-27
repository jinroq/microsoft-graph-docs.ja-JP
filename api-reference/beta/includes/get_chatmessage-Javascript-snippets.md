---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4d84c963bc4ecae3b3619e5ff5398cc37ce0f2d4
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35320280"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/chats/{id}/messages/{id}')
    .version('beta')
    .get();

```