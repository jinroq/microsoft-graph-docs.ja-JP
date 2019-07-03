---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5afd5578cd92ec9217f3afcf4a2181b15fd69329
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35503625"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const channel = {
  displayName: "Architecture Discussion",
  description: "This channel is where we debate all future architecture plans"
};

let res = await client.api('/teams/{id}/channels')
    .version('beta')
    .post({channel : channel});

```