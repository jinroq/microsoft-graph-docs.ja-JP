---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 98693fbf69f67a39cf214244030cfca4ea362993
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35527951"
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
    .update({domain : domain});

```