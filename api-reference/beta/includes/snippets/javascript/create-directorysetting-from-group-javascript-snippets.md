---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 210e402cfc4b97a03e44ec48e99a7ea4c787d224
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711792"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directorySetting = {
  directorySetting: {
    displayName: "displayName-value",
    templateId: "templateId-value",
    values: [
      {
        name: "name-value",
        value: "value-value"
      }
    ]
  }
};

let res = await client.api('/groups/{id}/settings')
    .version('beta')
    .post({directorySetting : directorySetting});

```