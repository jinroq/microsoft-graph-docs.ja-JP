---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 52bb5a9cabfc9a72c49eaccb735d0c82bf65c0ed
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713310"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directorySetting = {
  templateId: "templateId-value",
  values: [
    {
      name: "name-value",
      value: "value-value"
    }
  ]
};

let res = await client.api('/settings')
    .version('beta')
    .post({directorySetting : directorySetting});

```