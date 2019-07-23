---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 13688b6d23b33dc2c5ad44b0b962578d230429f6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722832"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  description: "Group with designated owner and members",
  displayName: "Operations group",
  groupTypes: [
    "Unified"
  ],
  mailEnabled: true,
  mailNickname: "operations2019",
  securityEnabled: false,
  owners@odata.bind: [
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ],
  members@odata.bind: [
    "https://graph.microsoft.com/v1.0/users/ff7cb387-6688-423c-8188-3da9532a73cc",
    "https://graph.microsoft.com/v1.0/users/69456242-0067-49d3-ba96-9de6f2728e14"
  ]
};

let res = await client.api('/groups')
    .post({group : group});

```