---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5e66a9672bbe19f45f66da263162ba2029673809
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721056"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  securityEnabledOnly: true
};

let res = await client.api('/contacts/{id}/getMemberGroups')
    .version('beta')
    .post(String);

```