---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 802a4cb4709d24a81590ccc68256e54b843ec872
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633329"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/chats/{id}/members/{id}')
    .version('beta')
    .get();

```