---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b304d194f254a7646e65c4fe9eb1561f936ad3d7
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637863"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  businessPhones: [
    "businessPhones-value"
  ],
  officeLocation: "city-value"
};

let res = await client.api('/me')
    .version('beta')
    .update(user);

```