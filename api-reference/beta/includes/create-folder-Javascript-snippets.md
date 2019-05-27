---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ca93721bc044ec34abd8b982215a4962c2efe700
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460890"
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