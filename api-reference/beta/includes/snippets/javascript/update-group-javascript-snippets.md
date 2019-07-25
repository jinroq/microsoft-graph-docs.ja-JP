---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6ad2c928c3d424429bef91270d6ed4ac1e39ebd9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711734"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  description: "description-value",
  displayName: "displayName-value",
  groupTypes: [
    "groupTypes-value"
  ],
  mail: "mail-value",
  mailEnabled: true,
  mailNickname: "mailNickname-value"
};

let res = await client.api('/groups/{id}')
    .version('beta')
    .update({group : group});

```