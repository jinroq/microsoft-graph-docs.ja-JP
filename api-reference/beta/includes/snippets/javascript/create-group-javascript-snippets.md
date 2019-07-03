---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6ea059da1fa82a97c6fb6b4b94729663f69929d3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526333"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  description: "Self help community for golf",
  displayName: "Golf Assist",
  groupTypes: [
    "Unified"
  ],
  mailEnabled: true,
  mailNickname: "golfassist",
  securityEnabled: false
};

let res = await client.api('/groups')
    .version('beta')
    .post({group : group});

```