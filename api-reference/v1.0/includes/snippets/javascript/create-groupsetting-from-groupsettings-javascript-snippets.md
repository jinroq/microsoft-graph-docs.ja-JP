---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 18cbef42fe72bd270fcdb2724c3ee70c0ff2c756
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741222"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const groupSetting = {
  displayName: "displayName-value",
  templateId: "templateId-value",
  values: [
    {
      name: "name-value",
      value: "value-value"
    }
  ]
};

let res = await client.api('/groupSettings')
    .post({groupSetting : groupSetting});

```