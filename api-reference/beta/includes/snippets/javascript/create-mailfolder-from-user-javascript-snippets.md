---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d25b43157517301d1d18edb0b0629fa7f06a0ee2
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637994"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  displayName: "displayName-value"
};

let res = await client.api('/me/mailFolders')
    .version('beta')
    .post(mailFolder);

```