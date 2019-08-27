---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a9c7b0266f5e735e14e35c066156ee33e0f90a9f
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637794"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const domain = {
  isDefault: true,
  supportedServices: [
    "Email",
    "OfficeCommunicationsOnline"
  ]
};

let res = await client.api('/domains/contoso.com')
    .version('beta')
    .update(domain);

```