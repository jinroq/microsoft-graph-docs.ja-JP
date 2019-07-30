---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f706b5ac082299520e0142d851d2ada51ba880be
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932860"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  name: "Just some files",
  "@name.conflictBehavior" : "rename",
  bundle: { },
  children: [
    { id: "1234asdf" },
    { id: "1234qwerty" }
  ]
};

let res = await client.api('/drive/bundles')
    .version('beta')
    .post({driveItem : driveItem});

```