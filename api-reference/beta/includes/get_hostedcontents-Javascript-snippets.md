---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c42adf7624b652005db3647b20b44319b1b31038
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35334105"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/chats/{id}/messages/{id}/hostedContents')
    .version('beta')
    .get();

```