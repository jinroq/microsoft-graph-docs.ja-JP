---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1c5c92a606d2877afdb7d99deb39740efaaa04ff
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637850"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const application = {
  allowPublicClient: false,
  displayName: "New display name"
};

let res = await client.api('/applications/{id}')
    .version('beta')
    .update(application);

```