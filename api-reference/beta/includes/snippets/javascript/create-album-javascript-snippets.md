---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 88f694de3bed843d5064d4d86e583606a4f03689
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637795"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  name: "My Day at the Beach",
  "@name.conflictBehavior" : "rename",
  bundle: { album: {} },
  children: [
    { id: "1234asdf" }
  ]
};

let res = await client.api('/drive/bundles')
    .version('beta')
    .post(driveItem);

```