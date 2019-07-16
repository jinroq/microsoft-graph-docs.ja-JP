---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9a676ca915ed4fd898beb9f17020c01ddc6086a6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738906"
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

let res = await client.api('/me/mailFolders/inbox/messageRules/AQAAAJ5dZqA=')
    .update({messageRule : messageRule});

```