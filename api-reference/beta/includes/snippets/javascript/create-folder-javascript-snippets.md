---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1e580696ee813523b2256ddccd34ca3c824d8087
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637791"
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
    .post(driveItem);

```