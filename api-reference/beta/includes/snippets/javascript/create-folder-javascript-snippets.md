---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ca93721bc044ec34abd8b982215a4962c2efe700
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712836"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  name: "New Folder",
  folder: { },
  @microsoft.graph.conflictBehavior: "rename"
};

let res = await client.api('/me/drive/root/children')
    .version('beta')
    .post({driveItem : driveItem});

```