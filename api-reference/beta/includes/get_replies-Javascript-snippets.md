---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9f765955a4fd0dac2977a816e8aa87fbb9378c4d
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35334485"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/chats/{id}/messages/{id}/replies')
    .version('beta')
    .get();

```