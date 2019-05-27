---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 97c87c7925e7f0a59468e4643f45f505b6b965f8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34476537"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const messageRule = {
    displayName: "Important from partner",
    actions: {
        markImportance: "high"
     }
};

let res = await client.api('/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')')
    .version('beta')
    .update({messageRule : messageRule});

```